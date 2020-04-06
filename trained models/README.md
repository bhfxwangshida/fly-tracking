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
  + sequence size 30, prediction size 10, RMSE better than v0.16, 1st error 0.0285,2nd error 0.0325, 3rd error 0.0375, 4th error 0.0418, 5th error 0.0471, 6th error 0.0513, 7th error 0.0567, 8th error0.0622 , 9th error 0.0685, 10th error 0.0746

* newmodel-32-64_seq30_pred10-v0.18
  + Uses temporal CNN instead of GRU. Sequence size 30, prediction size 10, RMSE much better than v0.17, 1st error 0.019, 10th error 0.086

* CNN-62-128_seq20_pred4-x-v0.21
  + sequence size 20, prediction size 4, 1st error 0.02582633386143601,2nd error 0.029721176201647187, 3rd error 0.03700379672647405, 4th error 0.04474210147333621

* GRU-32-64_seq20_pred4-y-v0.22
  + sequence size 20, prediction size 4, 1st error 0.0278,2nd error 0.0342, 3rd error 0.0419, 4th error 0.0498
  
* GRU-32-64_seq20_pred4-x-v0.22
  + 1st error 0.02360844694805981,2nd error 0.02968355305503326, 3rd error 0.0371320898808118, 4th error 0.04497059522528212
  
* CNN-62-32_seq30_pred4-x-v0.23
  + sequence size 30, prediction size 4, 1st error 0.027576247837159402,2nd error 0.03127663546590578, 3rd error 0.03856645353681183, 4th error 0.046221460408199244
  
* CNN-64-32_seq30_pred4-y-v0.23
  + sequence size 30, prediction size 4, 1st error 0.03489316616816865,2nd error 0.03671460584954812, 3rd error 0.0422472142226861, 4th error 0.04932160879630895
