# **On the impact of asynchronicity in stochastic gradient descent**

Optimization for Machine Learning course project.

Team members:
 - Nghia Nguyen Dai
 - Jean-Daniel Rouveyrol
 - Anthony Ducret

### **Abstract**
This study investigates the impact of the asynchronicity incorporated into stochastic gradient descent (SGD) on the optimization of large-scale models. Asynchronous SGD allows independent updates of model parameters based on gradient computed via each worker's fraction of the dataset. In contrast, synchronous SGD synchronizes model updates across all workers after each mini-batch to ensure consistent global updates. We conduct empirical evaluations and comparative analyses to examine the advantages, disadvantages, and trade-offs associated with both approaches. The study demonstrates that asynchronous SGD exhibits some regularization effects with a more pronounced result as the number of workers increases. However, it trade-offs in terms of slightly higher overall loss compared to synchronous SGD as well as the high sensitivity to the learning rate. The choice between the two methods depends on the specific requirements of the training scenario, considering factors such as training time, overall accuracy, and generalization. Further research is needed to explore convergence patterns and behaviors of different training variations, particularly with a higher number of workers.


### **Repo structure**
All of the experiments and visualizations for the main report could be reproduced using the `experiment.ipynb` notebook. Using regular Colab, the notebook could be run to reproduce the 4-work Async SGD. However, for a higher number of workers, a better runtime is required (Colab Pro).

The `save` directory store all the training logs from the experiment.