# LossLandscape
Explores the ideas presented in [Deep Ensembles: A Loss Landscape Perspective](https://arxiv.org/abs/1912.02757) by Stanislav Fort, Huiyi Hu, and Balaji Lakshminarayanan. 

In the paper, the authors investigate the question - ***why deep ensembles work better than single deep neural networks?*** 

In their investigation the authors figure out:

* Different snapshots (i.e. model from epoch 1, model from epoch 2, and so on) of a same model exhibit functional similarity. Hence, their ensemble is **less likely** to explore the different modes of local minimas in the optimization space. 
* Different solutions of a same model (i.e. trained with different random initializations each time) exhibit functional dissimilarity. Hence, their ensemble is **more likely** to explore the different modes of local minimas in the optimization space. 

Along with this fascinating finding, they present a number of different things that are useful to understand the dynamics of deep neural networks in general. To more about them check out our report. Huge to shoutout to **Yannic Kilcher** for making a stellar [explanation video of the paper](https://www.youtube.com/watch?v=5IRlUVrEVL8). It helped us accelerating our experimentation process. 
