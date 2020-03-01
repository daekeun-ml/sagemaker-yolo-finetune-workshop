# Finetune Person Tracker Worshop

This workshop is about how to use and finetune MXNet pretrained YOLO3 model for person tracking workload on AWS.

# Prerequisites

- AWS Account
- Basic knowledge of Machine Learning (especially what the hyperparmeter is and why it is important to Machine Learning)

# What each module is covering

- **00. MXNet YOLO3**(100) - In this module, we are going to find out how to use MXNet YOLO3 as multi-object-detector and make it detect person only.
After this module, you will get familiar with MXNet YOLO3.

- **01. DeepSORT**(200) - DeepSORT is one of the most famous multi object tracking framework.
In this module we are going to find out how to use DeepSORT with MXNet YOLO3 as people-object-tracker.
After this module, you will get mis-detected images by DeepSORT Tracker in your local storage.

- **02. Sagemaker Ground Truth**(200) - Ground Truth makes your labeling job easy.
With it you can label image bounding box or source.
In this module we are going to label mis-detected images with bounding box.
After this module, you will get 3 manifest files, such as `input.manifest`, `train.manifest` and `test.manifest` which are required to create Sagemaker Training Jobs.

- **03. Sagemaker HyperParameter Optimizer(HPO)**(300) - Finding Optimized HyperParamter Optimization is tedious job but very important also.
Sagemaker Hyperparameter Tuning Job will find the most optimized hyperparameter for your model automatically.
After this module, you will have a finetuned model, that is finetuned with the automatically selected hyperparameter, in S3 bucket.

- **04. Sagemaker Endpoint**(200) - Sagemaker Endpoint is the easiest way to serve your model on AWS, especially when you trained with sagemaker training job like HyperParameter Tuning Job.
After this module, you will get endpoint serving the model you finetuned with your own data.

- **05. Sagemaker Elastic Inference**(100) - Elastic Inference provides GPU acceleration to your endpoint. WIth EI, you can increase performance of the model and decrease the cost at the same time.
After this module, you will get EI enabled Sagemaker Endpoint.