# LossLandscape
Explores the ideas presented in [Deep Ensembles: A Loss Landscape Perspective](https://arxiv.org/abs/1912.02757) by Stanislav Fort, Huiyi Hu, and Balaji Lakshminarayanan. 

<div align="center">
<img src="https://i.ibb.co/NrR8KFJ/Untitled.png"></img>
</div>

In the paper, the authors investigate the question - ***why deep ensembles work better than single deep neural networks?*** 

In their investigation the authors figure out:

* Different snapshots (i.e. model from epoch 1, model from epoch 2, and so on) of a same model exhibit functional similarity. Hence, their ensemble is **less likely** to explore the different modes of local minimas in the optimization space. 
* Different solutions of a same model (i.e. trained with different random initializations each time) exhibit functional dissimilarity. Hence, their ensemble is **more likely** to explore the different modes of local minimas in the optimization space. 

Along with these fascinating findings, they present a number of different things that are useful to understand the dynamics of deep neural networks in general. To know more about them check out [our report](https://app.wandb.ai/authors/loss-landscape/reports/Understanding-the-effectivity-of-ensembles-in-deep-learning-(tentative)--VmlldzoxODAxNjA). 

## About the notebooks
- `*_CIFAR10.ipynb`: Shows the training process with three different  architectures (SmallCNN, MediumCNN, and ResNet20v1) as per the paper (with minor modifications).
- `*_Aug_Val_Acc_Ensembles.ipynb`: Investigates how accuracy can be represented as a function of ensemble size. 
- `Visualizing_Function_Space_Similarity_*.ipynb`: Investigates cosine similarity between weights collected from different snapshots and trajectories, prediction disagreement between different snapshots and trajectories, and presents tSNE visualizations of a how particular solution travels along the optimization landscape (not available for ResNet20v1). 

## Model weights
Available [here](https://github.com/ayulockin/LossLandscape/releases/tag/v0.1.0). 

## Acknowledgements

Thanks to **Yannic Kilcher** for [his amazing explanation video](https://www.youtube.com/watch?v=5IRlUVrEVL8) of the paper which helped us pursue our experiments. 

Thanks to **Balaji Lakshminarayanan** for providing feedback on the initial draft of the report and also for rectifying our mistake on the tSNE projections. 
