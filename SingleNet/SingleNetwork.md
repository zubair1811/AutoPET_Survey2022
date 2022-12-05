
|Research|Caner Type|Year|Backbone Model|IDE Tool|Optimizer|Batch Size|Epochs|Loss Function|GPU|Baseline|Cross-Tersting|Whole-body|Cross-Validation|Futurte Direction   |
|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:-----------:|
|zhong2019simultaneous|NSCLC|2019|3D U-Net|TensorFlow|Adam|4|21|PW_CE + Dice|GTX 1080Ti|Y|N|Y|5-Fold|Validation of the PET/CT segmentation on other datasets including multi-institutional trials and more different neural network architectures will also be investigated in the future|
|moreau2021automatic|Breast |2022|3D U-Net|PyTorch|SGD|250|1000|Multi-class dice + CE|GTX 1080Ti|N|Y|N|5-Fold|Small Dataset of 60 patients|
|xu2018automated|Multiple myeloma |2018|3D V-Net|Theano|Adam|--|--|CE|GTX |--|N|Y|3-Fold|the current study is restricted by small number of patient data.|
|iantsen2020squeeze|H&N |2021|U-Net|--|Adam|2|800|Soft Dice Loss, Focal Los|GTX 1080Ti (x2)|--|Y|N|LOCO|---|
|xie2020head|H&N |2021|3D U-Net|PyTorch|SGD|2|250|Weighted CE + Dice|RTX 2080Ti|Y|Y|N|--|we will investigate the impact of different data partitions on the model performance such as leave-one-center-out as test data, Large inference time than nnUNet|
|kot2021u|Brain |2021|U-Net|TensorFlow|Adam|32|50|BCE|Telsa V100|Y|--|--|5-Fold|Less data of 20 patients, Early fussion |
|zhao2018tumor|NSCLC |2019|3D FCN|TensorFlow|Adam|--|350|Weighted CE|GTX 1080Ti|Y|--|N|Random|Image cropping to ROI, Donain shift challenge, Weight parameters adjust manually |
|groendahl2021comparison|H&N |2021|CNN|TensorFlow|Adam|--|200|Evidence Loss|GTX 1080Ti|Y|--|N|5-Fold|---|
|zhong20183d|NSCLC |2018|3D U-Net|TensorFlow|Adam|1|20|CE, dice|GTX 1080Ti|Y|N|N|--|small Dataset of 32 patients|
|li2020deep|NSCLC |2020|FCN|TensorFlow|Adam|1|350|--|GTX 1080Ti|Y|N|N|--|---|
|kumar2019co|NSCLC |2020|CNN|TensorFlow|SGD|5|500|Modified CE|GTX 1080Ti|Y|N|N|3-Fold|More Focus on fusion than segmentation result, can be improved using Rsidual or Insception concept, focuds on specific body part, manual process required to constract dataset for model, same coordinate space requireed|
|zhao2019automatic|NPC |2019|FCN|Matconvnet|Adam|--|--|CE|Titan X|N|N|Y|5-Fold|A disadvantage of our method is that the dataset is limited, such that an outlier appears. Another deficiency is that sequential information between consecutive slices was not utilized when we separated a 3D image into many 2D slices|
|andrearczyk2020automatic|H&N |2020|U-Net|NiftyNet|Adam|12|200|Dice + CE|Tesla V100|N|Y|N|LOCO|An automatic pipeline to detect the oropharyngeal region in a full body scan will also be developed to bypass the limitation of the proposed approach that centers input volumes around the tumors.|
|xue2021multi|Liver |2021|V-Net|PyTorch|Adam|1|300|Focal Tversky+ Similarity|Tesla V100|Y|N|N|10-Fold|Misses information from some tiny lesions,  In addition, the need for the liver contour segmentation increases the model size and requires fine morphological postprocessing|
|biase2021skip|H&N |2022|V-Net|PyTorch|Adam|--|--|BCE + Dice|Tesla V101|--|Y|N|5-Fold|Our methods may not perform well on some cases in which we have low FDG uptake on PET, or when the primary tumor can be confused with a lymph node, or when the tumor is present at the border of the oropharynx region|
|yuan2021diffuse|DLBCL |2021|CNN|TensorFlow|SGD|--|--|BCE|RTX 2080Ti|Y|N|N|15-Fold|Create Baseline witgh same structure of network.  our method required the manual selection of the volume contained DLBCL lesions so its cross sections could form the CNN inputs with the guarantee of correct bodyregion data set. Does not deal with spatial fusion for different resolution images|
|huang2022multi|DLBCL |2022|3D V-Net|TensorFlow|Adam|--|150|CE+Dice, regularization|--|Y|--|--|--|---|
|xu2021disegnet|DLBCL |2021|SegNet|--|Adam|--|200|cosine-sine|--|--|--|--|4-fold leave-10-cases out validation|---|
|wang2022psr|Lymphoma |2022|3D U-Net|TensorFlow|Adam|1|100|weighted focal + weighted Dice |GTX 1080Ti|--|--|Y|5-Fold|---|
|xiang2022modality|NSCLC |2022|Encoder-Decodre|--|Adam|1|110|adversarial|RTX 3090|Y|--|--|--|Test on two lung cancer daatset|
|bi2021recurrent|NSCLC |2021|ResNet|PyTorch|Adam|5|300|PW_CE + Dice|RTX 2080Ti|--|--|--|5-Fold|---|
|huang2022isa|H&N |2022|3D U-Net|--|Adam|1|300|Focal + dice|RTX 3090|--|--|--|5-Fold|model was complex and the computational cost was high|
