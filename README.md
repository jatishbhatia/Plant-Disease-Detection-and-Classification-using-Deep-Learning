# A CNN based image classification of Plant diseases
## Datasets
1. Cassava Dataset [https://tensorflow.google.cn/datasets/catalog/cassava]: The Cassava dataset features leaf images of the cassava plant, showcasing healthy leaves and four disease conditions: Cassava Mosaic Disease (CMD), Cassava Bacterial Blight (CBB), Cassava Green Mite (CGM), and Cassava Brown Streak Disease (CBSD). It includes 9,430 labeled images

2. Crop Pest and Disease Dataset [https://data.mendeley.com/datasets/bwh3zbpkpv/1]: This dataset, obtained from local farms in Ghana, is composed of two parts: raw images totaling 24,881, divided into 22 classes. These images are distributed among four types of crops as follows: 6,549 images of Cashew, 7,508 of Cassava, 5,389 of Maize, and 5,435 of Tomato.[2]

3. PlantVillage Dataset [https://www.tensorflow.org/datasets/catalog/plant_village]: The PlantVillage dataset features 54,303 images, showcasing both healthy and diseased leaves, organized into 38 distinct categories according to plant species and disease type.

## Install Dependencies
Run the below command to install all the dependencies:

```
pip install -r requirements.txt
```


## Usage
Run the below command to run entire pipeline or just inference pipeline:

```
python main.py --dataset [dataset] --model [model] --train_mode [True/False] --pretrained [True/False] --max_epochs [max_epochs] --batch_size [batch_size] --lr [learning rate] --tune_hyperparams [True/False]

dataset: cassava, crop_diease, plant_village
model: googlenet, efficientnet_b0, mobilenet_v2
train_mode: True for running in training else False
pretrained: True for using pre-trained weights else False
max_epochs: number of epochs
batch_size: batch size
lr: learning rate
tune_hyperparams: True for tuning hyperparams else False
```
