# What is Synapse Open Dataset?
Synapse Open Dataset is a multi-view camera dataset that is especially targeted at warehouse autonomous mobile robots (AMRs). This dataset is created using Isaac simulator from Nvidia.

## Paper:
Synapse Open Dataset v1: Multi-view cameras in 74.8*36 m^2 warehouse. Link coming up soon.

## Dataset:
[Dataset_v1](https://drive.google.com/drive/u/3/folders/1NZjuwP6osCelOG8H9QNm9wooHqaO4VKm): Multi-view camera images with annotations as instance/ semantic segmentation, 2D/ 3D bounding boxes, surface normal estimation, dense-depth estimation. 
```
pip install gdown
gdown 1r_yl1CNzIlOi-Kn-ieQSUDtUSFDCI_56
```

## Warehouse Scenario
Perspective view of a scene in the USD (Universal Scene Description) warehouse. 
<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/ead2c00a-7fcf-4731-b279-5c7ce453712e">

## Available Annotations
* Dense Depth Estimation
* 3D/ 2D Detection Bounding Boxes
* Surface Normal Estimation
* Instance/ Semantic Segmentations
  
<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/14a682b1-a9ff-40f5-b88c-17908872b5ec">

## BEV view of the Warehouse
Full BEV view of the first version of the dataset showing multiple columns and rows as aisles, along with a 2D BEV map on top-right. 

<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/72b44af2-1053-4575-83b6-b3280a359fe1">

* * *
# Diverse Scenarios
We curated this dataset based on multiple site visits to the warehouse to minimize the real-world and synthetic data domain gap. It contains various assets that mimic any real-world warehouse. Sample meta_data.json:
```
{
    "warehouse_version": "v2", 
    "dataset_version": "0.0.1",
    "modality": "camera_only",
    "camera_list": ["cam_front", "cam_right", "cam_left", "cam_back"],
    "random_lighting": true,
    "forklifts": false, 
    "humans": false, 
    "misc_warehouse_items": false,
    "robots": false
}
```

### Randomness in Lighting
<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/a4da071d-ad52-4c55-9973-ef12afc322ff">


### Randomness in Humans
<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/52f49d99-c19f-4576-9f0f-018cb1bf0e43">


### Ramdomness in Forklifts

<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/f285067c-ef7c-41af-9386-756d35dd7ae9">

### Randomness in other Robots

<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/c8f28878-062a-4e22-8896-bef0bac0ac04">


### Randomness in Misc. Warehouse items

<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/6e00b23b-9fae-40c2-85e0-45996ccaf9c7">


### Randomness in Shelves

<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/850795a9-9389-4dd3-b28b-d21326bcdc6c">


# Sensors Suite
<img width="800" alt="image" src="https://github.com/synapsemobility/synapse_open_dataset/assets/163760520/3ad9a5d7-f721-4a42-9985-72b5f6bea9a5">



# How to cite

If you are using this dataset, please cite using:

```
@article{singhsynapse,
  title={Synapse Open Dataset: A dataset for warehouse robots},
  author={Singh, Apoorv and Choudhary, Alka}
}
```
