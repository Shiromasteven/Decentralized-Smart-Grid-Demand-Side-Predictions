# Applying Optimized Machine Learning Algorithms for the Prediction of Decentralized Smart Grid Stability

## A demand side approach to power grid monitoring

By:Steven Shiroma

### Business Problem:
Centralized power grids as an energy infrastructure are vulnerable and slow to adapt to changing fluctuations in supply and demand of renewable energy sources, and as well the future of prosumers, consumers on the energy grid who also provide power back into the system via solar energy for example. By using an optimized machine learning algorithm demand side, consumers are able to react very quickly to changing energy ecosystems, allowing for the adaptability of smart homes to adjust their consumption of energy automatically by monitoring the fluctuations the existing energy infrastructure and by the nature of those fluctuating frequencies determine during surplus or deficit, how best to reduce consumption or to in the case of prosumers, supply energy back to the grid for more accurate profit.

### Data:
Data source is located in the UCI Machine learning repository [here](https://archive.ics.uci.edu/ml/datasets/Electrical+Grid+Stability+Simulated+Data+#) 

### Methods:
- Very little data cleaning was necessary however the features 'stab' and the target feature 'stabf' are directly related and therefor dropped 'stab'
- For the data engineered data frame each of the three 'nodes', 'tau2, tau3, tau4' etc. was averaged and consolidated into one feature each giving purely a producer and consumer feature.
- For the PCA Model of each version features where reduced down to only 2 to maintain variance.


### Models
