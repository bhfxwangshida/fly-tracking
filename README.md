# fly-tracking
## v0.02
network structure 32-64-64-64, only support one sample, no data preprocessing, MSE 0.03.
## v0.03
network structure 32-64-64-64, combine two samples,no data preprocessing, MSE 0.03.
## v0.04
network structure 32-64, multiple samples, data preprocessed, MSE 0.11(with early stopping patience=20), MSE 0.07(without searly stopping, epoch 1000).
## v0.05
network structure 32-64, 89000 samples, data preprocessed, earlystopping 100, sequence size 10, seperate x and y training into two seperate model.
