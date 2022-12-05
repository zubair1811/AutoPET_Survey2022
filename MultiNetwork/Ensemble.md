|Research|Caner Type|Year|Backbone Model|IDE Tool|Optimizer|Batch Size|Epochs|Loss Function|GPU|Baseline|Cross-Tersting|Whole-body|Cross-Validation|Futurte Direction   |
|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:-----------:|
|chen2020iteratively|H&N |2020|3D UNet|---|Adam|---|50|Dice|---|N|Y|N|---|---|
|qayyum2021automatic|H&N |2022|3D ResNet, Inception|PyTorch|Adam|2|100|Dice + BCE|---|Y|Y|N|5-Fold|---|
|wang2021hd|lymphoma |2022|U-Net|TensorFlow|Adam|1|100|weighted Dice|Tesla V100|Y|N|Y|five-fold patient independent |---|
|huang2021deep|lymphoma |2020|U-Net|TensorFlow|Adam|---|---|Dice + MS |Tesla V100|Y|N|Y|---|Ignore the combine uncertain information|
|jemaa2020tumor|lymphoma, NSCLC |2022|U-Net|---|RMSProp|16|25|Dice + WCE|Quadro P6000|N|N|Y|---|---|
|amiri2022improved|lymphoma, NSCLC, Melanoma |2022|U-Net|PyTorch|Adam|2/1|30000|Dice + CE |RTX 3080|N|Y|Y|---|---|
|sibille2022whole|lymphoma, NSCLC, Melanoma |2022|U-Net|PyTorch|AdamW |---|200|Dice + CE + sensitivity |Tesla V100|N|Y|Y|---|---|
