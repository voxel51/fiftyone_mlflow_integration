# <span style="color: #ff6D04; font-weight: bold;">MLflow + FiftyOne Integration</span>


![MLflow](./assets/mlflow.gif)

Welcome to the demo repoistory of an example workflow of MLflow integrated into the FiftyOne App!

The repo consists of two main parts: 
1. The yolov9 submodule, a forked repository from the orignial repository that now also includes MLflow hooks in a custom training script. Make sure to run the following to initialize the repo: 
```
git submodule init
git submodule update
```
2. [The FiftyOne + MLFlow plugin](https://github.com/jacobmarks/fiftyone_mlflow_plugin), a FiftyOne plugin that brings MLFlow UI in the app as a panel, as well as track experiments and runs across your FiftyOne datasets. The plugin can be installed with:
```
pip install fiftyone mlflow
fiftyone plugins download https://github.com/jacobmarks/fiftyone_mlflow_plugin
```

## Running the Demo

To run the example demo, first download the test dataset. We will be using a subset of [VisDrone](https://github.com/VisDrone/VisDrone-Dataset), a top of line drone dataset. We will only be looking at the trainset as an example and the direct downlink from Google Drive can be found [here](https://drive.google.com/file/d/1a2oHjcEcwXP8oUF95qiwrqzACb2YlUhn/view).

Once the repo is cloned and the dataset downloaded, you can run the [jupyter notebook](mlflow_fiftyone_workflow.ipynb). The notebook serves as a guided journey of an example workflow of monitoring and evaluating the training of models with FiftyOne and MLflow.

## Helpful Links

Here are some helpful links to resources or tools used within the notebook.

### Plugins
- [Find image quality issues](https://github.com/jacobmarks/image-quality-issues)
- [Find exact and approximate duplicates](https://github.com/jacobmarks/image-deduplication-plugin)
- [Find outliers in your dataset](https://github.com/danielgural/outlier_detection) 
- [Compare one model to another](https://github.com/allenleetc/model-comparison)

Find all the other FiftyOne Plugins [here](https://github.com/voxel51/fiftyone-plugins)!


### FiftyOne Brain
- [Visualize embeddings with FiftyOne Brain](https://docs.voxel51.com/user_guide/brain.html#visualizing-embeddings)
- [Search your datasets with text prompts or sort by similarity](https://docs.voxel51.com/user_guide/brain.html#similarity)
- [Sort by uniqueness](https://docs.voxel51.com/user_guide/brain.html#image-uniqueness)

### YOLOv9

- [Original Yolov9 Repo](https://github.com/WongKinYiu/yolov9)