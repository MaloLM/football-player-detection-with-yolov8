# Football Player Detection with YOLO

A basic starting in computer vision including YOLO finetuning for a specific task.

Finetuning based onto following [HuggingFace football dataset](https://huggingface.co/datasets/keremberke/football-object-detection).


# References

https://huggingface.co/Ultralytics/YOLOv8

https://docs.ultralytics.com/usage/python/

https://docs.ultralytics.com/modes/train/

https://www.youtube.com/watch?v=ZUhRZ9UTkIM

https://www.youtube.com/watch?v=wuZtUMEiKWY

https://docs.ultralytics.com/models/yolov9/

https://machinelearningspace.com/coco-dataset-a-step-by-step-guide-to-loading-and-visualizing/

https://stackoverflow.com/questions/75268393/yolov8-how-does-it-handle-different-image-sizes

https://umvie.com/guide-complet-sur-le-format-yolo-bbox-tout-ce-que-vous-devez-savoir/

https://github.com/ultralytics/ultralytics/issues/1270#issuecomment-1550179877

https://y-t-g.github.io/tutorials/yolov8n-add-classes/

conda install -c conda-forge ultralytics


conda remove --name tf-wsl --all


https://github.com/MaloLM/jupyter-ml-with-GPU-support/blob/main/setup.md#setting-up-your-conda-virtual-environment

https://docs.ultralytics.com/yolov5/tutorials/tips_for_best_training_results/


What I have learn from this project ?

- model requires a lot of data from the most perspectives possible. Classes having very few samples will be of course poorly detected and sometimes even missclassifyed.

- I have learned how to use the Ultralytics YOLOv8 framework which will be usefull for many other usecases such as image segmentation, pose estimation, object tracking and image classification

- It motivates me to commit myself in CNN model performances optimisation for being able to cover most of the CNN usecases, such as embedded computer vision.