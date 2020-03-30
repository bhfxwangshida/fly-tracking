# fly‘s track prediction
* v0.02
+ network structure 32-64-64-64, only support one sample, no data preprocessing, MSE 0.03.
* v0.03
+ network structure 32-64-64-64, combine two samples,no data preprocessing, MSE 0.03.
* v0.04
+ network structure 32-64, multiple samples, data preprocessed, MSE 0.11(with early stopping patience=20), MSE 0.07(without searly stopping, epoch 1000).
* v0.06
+ network structure 32-64, 89000 samples, data preprocessed, earlystopping 100, sequence size 10, seperate x and y training into two seperate model. y-test sample: 20200109_195406-5\\clip5, test MSE 0.027, train MSE 0.02570. model name newmodel-32-64_850-y-v0.06.
* newmodel-64-128_850-v0.06
+ patience 100, RMSE worse than 0.07
* newmodel-64-128_850-v0.07
+ test RMSE 0.027 train RMSE 0.022, patience 300
* newmodel-32-64_seq30_pred6-v0.16
+ sequence size 30, prediction size 6
* newmodel-32-64_seq30_pred10-v0.17
+ sequence size 30, prediction size 10, RMSE better than v0.16
