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

###Results
#### Volume of Energy Consumed or Produced
![Volume of Energy Consumed or Produced](https://user-images.githubusercontent.com/95104650/181662211-c1e9a74e-7fd5-475d-996a-06fc32d6a0b6.png)

- A key insight to the decentralized energy grid is it's desire to be near equilibrium. In this graphic the total of production was averaged, and the three features of consumption averaged and stacked.

#### Stable Ranges of Operation
![Stable_ranges_of_Operation](https://user-images.githubusercontent.com/95104650/181664187-2fe90e55-b018-49b8-a2e7-41bad878b7fb.png)

- Here we can see the operant conditions and the peak operating stability conitions of the system.


###Model

- My final model consists of a tuned Random Forest model. My decision to use the random forest was dervied from it's ability to produce accurate results from non linearly correlated data and achieved a...

-Precision of 91%

-Recall of 89%

-F-1 of 89%

![Final Model Confusion Matrix](https://user-images.githubusercontent.com/95104650/181672223-815ead08-2d0e-4638-883a-68f8c2340e5d.png)

- By having a high accuracy and low chance of false positives, the model will more accurately predict when the system is likely to fail prompting more accurate timings of energy usage and restrictions.



### Limitations and Next Steps

- This model is of course limited to the synthetic nature of the data set, but it is the proof of concept that an optimized random forest model could be used in a real world test case of a decentralized power grid to provide demand side predictions of decentralized power grids.

- Of course the next step would be to evaluate this sort of model on real world test cases!

### Further Information
