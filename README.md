# Football Player Detection with YOLO

This project demonstrates the use of Ultralytics YOLOv8 for a specific task: detecting football players in images. The project includes the entire process, from dataset preparation to model testing, including training and validation.

![demo](./demo_gif.gif)

## Dataset

The dataset used for this project is the [HuggingFace football dataset](https://huggingface.co/datasets/keremberke/football-object-detection). This dataset contains images of football matches, with annotations indicating the location and size of football players and the ball in each image.

## Environment Recommendations

To ensure the project runs smoothly, it is recommended to use a fresh Python virtual environment (venv) with Python 3.9. The project has been tested on Windows 11 with WSL2, and it is likely to work on Linux distributions as well.

It is recommended to use a base Python venv instead of a conda venv, as the Ultralytics ecosystem works better through pip than conda. This can help to avoid package version issues.

The project uses JupyterLab with notebooks, but it is not recommended to use Ultralytics technologies through a notebook, as many display features such as camera streaming and live inference are not displayable from inside a notebook.

If you prefer to use YOLO through a conda install, you can use the following command to install it from the conda-forge channel:

```
conda install -c conda-forge ultralytics
```

Key Learnings and Future Directions

- **Data Requirements**: The model requires a large amount of data from various perspectives to perform well. Classes with few samples may be poorly detected or even misclassified.
- **Ultralytics YOLOv8 Framework**: I have gained experience in using the Ultralytics YOLOv8 framework, which will be beneficial for future use cases such as image segmentation, pose estimation, object tracking, and image classification, as well as heatmaps.
- **Model Optimization**: The project has motivated me to focus on optimizing CNN model performance to cover most CNN use cases, such as embedded computer vision.
- **Dataset Limitations**: The dataset used in this project is relatively small, which led to the "ball" class having very few annotations. This resulted in sport balls being detected only in the context in which they were annotated. For example, balls are hardly detected inside the cage or under shadows... Data is the model.

## Improvements

- **Expand the Classes**: Adding more classes to the model, such as referee, goal cage, and goal keeper, could improve make the model even more usefull.
- **Increase the Dataset Size**: Adding more annotated data to the dataset could help to improve the model's accuracy and robustness.
- **Use Online Football Videos as Test Set**: Instead of using a separate test dataset, merging the test data into the training dataset and using online football videos as the test set could provide a more realistic evaluation of the model's performance in real-world scenarios. This could also increase the training data size, which is currently limited.

## References

- Ultralytics YOLOv8 Documentation: <https://huggingface.co/Ultralytics/YOLOv8>
- Ultralytics Python Usage Documentation: <https://docs.ultralytics.com/usage/python/>
- Ultralytics Training Mode Documentation: <https://docs.ultralytics.com/modes/train/>
- YOLOv8 Tutorial by Ultralytics: <https://www.youtube.com/watch?v=ZUhRZ9UTkIM>
- YOLOv8 Training Tutorial by Ultralytics: <https://www.youtube.com/watch?v=wuZtUMEiKWY>
- Ultralytics YOLOv9 Documentation: <https://docs.ultralytics.com/models/yolov9/>
- COCO Dataset Guide: <https://machinelearningspace.com/coco-dataset-a-step-by-step-guide-to-loading-and-visualizing/>
- StackOverflow: YOLOv8 Handling Different Image Sizes: <https://stackoverflow.com/questions/75268393/yolov8-how-does-it-handle-different-image-sizes>
- Understanding YOLO BBox Format: <https://umvie.com/guide-complet-sur-le-format-yolo-bbox-tout-ce-que-vous-devez-savoir/>
- Ultralytics Issue: Adding Custom Classes to YOLOv8: <https://github.com/ultralytics/ultralytics/issues/1270#issuecomment-1550179877>
- Adding Custom Classes to YOLOv8 Tutorial: <https://y-t-g.github.io/tutorials/yolov8n-add-classes/>
- Setting Up Jupyter ML with GPU Support: <https://github.com/MaloLM/jupyter-ml-with-GPU-support/blob/main/setup.md#setting-up-your-conda-virtual-environment>
- Tips for Best Training Results with YOLOv5: <https://docs.ultralytics.com/yolov5/tutorials/tips_for_best_training_results/>