# DRO-Deep-Kernel-Multiple-Instance-Learning
This is the code for the paper "Distributionally Robust Optimization for Deep Kernel Multiple Instance Learning". 
Processed dataset required for the training will be provided separately in the google-drive because of the size issue.
We have evaluation on five different datasets in the paper: (1) SanghaiTech, (2) UCF-Crime, (3) Avenue, (4) SanghaiTech Outlier, and (5) UCF-Crime Multimoal.

## SanghaiTech Dataset:
To train the model for SanghaiTech Dataset execute the following command:
python train_mil_sanghaitech.py split_no rep_no eta


## UCF-Crime Dataset:
To train the model for UCF-Crime Dataset, execute the following command:

python train_mil_ucfcrime.py rep_no eta

## Avenue Dataset:
To train the model for Avenue Dataset, execute the following command:

python train_mil_avenue.py cv_no rep_no eta

## SanghaiTech Outlier Dataset:
To train the model for SanghaiTech Outlier Dataset, execute the following command:

python train_mil_sanghaitech_outlier.py split_no rep_no eta

## UCF-Crime Multimodal Dataset:
To train the model for UCF-Crime Dataset, execute the following command:

python train_mil_ucfcrime_multimodal.py rep_no eta

Where; 
### rep_no: Replication number we considered during training. If we want to run the model for different random initialization, we can call with different rep_no
### eta: Hyperparameter considered in the training for DRO framework (10^-8-1.0)
### split_no: validation-test pair for sanghaitech and sanghaitech outlier dataset (1, 20)
#### cv_no: cross validation number considered in the Avenue dataset. We have 5 pairs of training-testing set (1-5)



