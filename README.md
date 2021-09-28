# Build an ML Pipeline for Short-Term Rental Prices in NYC

This project show cases a ML pipeline.

To run the entire pipeline, run:
```
mlflow run .
```

To run a specific step, run:
```
mlflow run . -P steps=test_regression_model
```

The possible steps are:
```
download
basic_cleaning
data_check
data_split
train_random_forest
test_regression_model
```

To run remotely with new data, run:
```
mlflow run https://github.com/akionakamura/nd0821-ml-pipeline.git -v 1.0.1 -P hydra_options="etl.sample='sample2.csv'"
```

The Weights and Biases experiment tracking can be found here: https://wandb.ai/akionakas/nyc_airbnb
