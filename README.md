
# RSNA-MICCAI Brain Tumor Radiogenomic Classification

## Training
4 models were trained with 1 MRI type each, and ensembled. All models were 3D EfficientNet models and were trained with the following settings:
    * `IMG_SIZE`: 256
    * `optimizer`: Adam with lr=0.001 and early stopping
    * `loss function`: binary cross entropy loss
    * `metric`: roc_auc
    * `epochs`: 10
An ensembled model reached `roc_auc_score of 0.64`.