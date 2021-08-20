
## Tutorial code for 2D density estimation and energy matching (variational inference)
  >


## Requirements
* **``python>=3.6``** (it will probably work on older versions but I have not tested on them)
* **``pytorch>=1.0.0``**
* **``FrEIA 0.2``**

For ``FrEIA`` development:

####  first clone the repository
git clone https://github.com/VLL-HD/FrEIA.git
####  then install in development mode, so that changes don't require a reinstall
cd FrEIA
python setup.py develop

Optional for visualization and plotting: ``numpy``, ``matplotlib`` and ``tensorboardX``


--- 
### Run 2D toy density estimation
This example runs density estimation on the `8 Gaussians` dataset using 1 flow of BNAF with 2 layers and 100 hidden units (`50 * 2` since the data dimensionality is 2).
```
python toy2d.py --dataset 8gaussians \    # which dataset to use
                --experiment density2d \  # which experiment to run
                --flows 1 \               # BNAF flows to concatenate
                --layers 2 \              # layers for each flow of BNAF
                --hidden_dim 50 \         # hidden units per dimension for each hidden layer
                --save                    # save the model after training
                --savefig                 # save the density plot on disk
```

![Imgur](https://i.imgur.com/DWVGsyn.jpg)

### Run 2D toy energy matching
This example runs energy matching on the `t4` function using 1 flow of BNAF with 2 layers and 100 hidden units (`50 * 2` since the data dimensionality is 2).
```
python toy2d.py --dataset t4 \            # which dataset to use
                --experiment energy2d \   # which experiment to run
                --flows 1 \               # BNAF flows to concatenate
                --layers 2 \              # layers for each flow of BNAF
                --hidden_dim 50 \         # hidden units per dimension for each hidden layer
                --save                    # save the model after training
                --savefig                 # save the density plot on disk
```

![Imgur](https://i.imgur.com/o1QR3XO.jpg)

#### BNAF paper  
Pytorch implementation of Block Neural Autoregressive Flow based on our paper:
> De Cao Nicola, Titov Ivan and Aziz Wilker, [Block Neural Autoregressive Flow](http://arxiv.org/abs/1904.04676) (2019)
