
|Research|Caner Type|Year|Backbone Model|IDE Tool|Optimizer|Batch Size|Epochs|Loss Function|GPU|Baseline|Cross-Tersting|Whole-body|Cross-Validation|Futurte Direction   |
|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:-----------:|
|li2019densex|lymphoma |2020|FC-DenseNet|TensorFlow|Adam|---|---|Dice + focal|GTX 1080Ti|N|N|Y|5-Fold|---|
|meng2021multi|H&N  |2022|U-Net|TensorFlow|Adam|8|10000|Dice + logarithm partial likelihood|---|N|Y|N|5-Fold|---|
|meng2022deepmts|NPC |2022|3D U-Net|TensorFlow|Adam|8|15000|Dice + logarithm partial likelihood|Titan X|N|N|N|5-Fold|A larger dataset is desired for further validation and potentially enables better performance|
|andrearczyk2022segmentation|H&N  |2022|U-Net|TensorFlow|Adam|4|200|Dice + batchaggregated dice|V100|N|Y|N|5-Fold|---|
|blanc2021fully|lymphoma |2020|3D U-Net|PyTorch|SGD|---|---|CE + Dice |GTX 1080Ti|N|Y|Y|5-Fold|Pre-processing required which loss the information. Onley one expert anonaste the the that which lead to inter variability challenge. Used the 41% threshold for SUV which limit the variability|
|qayyum20223d|H&N  |2022|Encoder-Decoder|PyTorch|Adam|2|1000|BCE + Dice|---|Y|Y|N|5-Fold|we have used discrete intervals based on observations in the training data, excule some clinical feratures. our system is built on Inception based framework, which is not designed to handle CT and PET data|
|qayyum2023semi|H&N |2023|Encoder-Decoder|PyTorch|Adam|2|1000|BCE + Dice|---|Y|Y|N|5-Fold|---|

