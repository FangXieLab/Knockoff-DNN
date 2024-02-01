# Knockoff-based-False-Discovery-Rate-Control-for-Deep-Neural-Networks-and-Simplify-Neuron-Networks
The deep neural network stands out as a widely adopted framework in machine learning, extensively utilized in diverse fields. However, deep neural network often encompass an abundance of parameters and inputs, and many of these may prove irrelevant to the target or output. And these parameters and inputs not only increase computational complexity but also contribute to add computational costs.
The knockoffs methods are a solution of this problem, which have demonstrated success in controlling false discovery rates in high-dimensional regressions. Building upon the knockoffs methods and leveraging the neural network regularization loss function, this paper proposes three variable screening methods under the condition of controlling the false discovery rates:
one layer filter: Screens variables based solely on the regularization parameters of each weight in the first layer of the network.
multiple layers filter: Combines the regularization parameters of weights in the first layer with all weights to filter variables.
and variable weight accumulation filter: Utilizes different neural network models with distinct activation functions and employs hard voting to filter variables.
Additionally, based on the regularization parameters of each weight obtained during variable screening, we also proposed an algorithm called \textit{reduced weight} to simplify the structure of neural networks. Through algorithms simulation and application, and in comparison with existing algorithms, we found that our algorithms exhibit satisfying performance.

## For 'Simulation' file:
``One layer and Multiple layers filters.ipynb``: simulate our algorithms with one layer and multiple layers filter.
``Optimization and VWA filter(1).ipynb``: simulate our algorithms with optimizers and VWA filter in different related variables.
``Optimization and VWA filter(2).ipynb``: simulate our algorithms with optimizers and VWA filter in different network structures and distributions.
``Prediction.ipynb``: use fitered results to predict the dependent variable.

## For 'Application' file:
``One layer and Multiple layers filters.ipynb``: use one layer filter, multiple layers filter to select the related variables of breast-cancer.
``Optimization and VWA filter.ipynb``: use optimizers and VWA filter to select the related variables of breast-cancer.
``Prediction.ipynb``: use the screened results to predict the breast-cancer.
``Variations Distribution.ipynb``: visualize the selected variations to find the explanation of the result.

## For 'Other models' file:
Here we use ``deepPINK``, ``deepLINK``, ``Linear model-knockoff`` to fiter varibles, use the selected results to compare with the results filtered by our algorithms.

The data we use in the application.[link][cancer.csv]

Code/
│
├── Simulation/
│   ├── One layer and Multiple layers filters.ipynb
│   └── Optimization and VWA filter(1).ipynb
│   └── Optimization and VWA filter(1).ipynb
│   └── Prediction.ipynb
│
├── Application/
│   ├── One layer and Multiple layers filters.ipynb
│   └── Optimization and VWA filter.ipynb
│   └── Prediction.ipynb
│   └── Variations Distribution.ipynb
│
└── Other model/
    ├── deepPINK
    └── deepLINK
    └── Linear model-knockoff
