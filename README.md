# mlops_project


#### Kabir Patel

os.environ["MLFLOW_TRACKING_URI"] = "https://dagshub.com/kabirpatel1203/mlops_project.mlflow"
os.environ["MLFLOW_TRACKING_USERNAME"] = "kabirpatel1203"
os.environ["MLFLOW_TRACKING_PASSWORD"]="7fd977a05dfc244e0090d7fbed872ac1daf8bc47"




# Project Summary

In this project, I'm implementing an end-to-end deep learning solution for a chest cancer detection system using MLOps tools like MLflow and DVC, as well as Docker for containerization. The goal is to build and deploy a deep learning model that can accurately detect the presence of chest cancer from medical images. To accomplish this, I'm leveraging MLOps and Docker practices and tools to streamline the development and deployment process.


I start by setting up a virtual environment and installing all the necessary packages, including those required for computer vision and deep learning. Next, I build a logging and utility module, which is crucial for debugging and maintaining the codebase. I create a logging function within my chest cancer detection CNN classifier code.
Moving on to configuration management, I use a tool called ConfigBox to handle all my project settings, such as the dataset paths, model hyperparameters, and deployment configurations. This makes it much easier to maintain and update the project settings as needed. I then extract file IDs from Google Drive URLs and download the medical image dataset using MLflow and DVC.


With the data in place, I create a data initialization pipeline using MLflow and DVC. This helps me set up the data preprocessing and augmentation steps in a structured, version-controlled way. I then implement the full end-to-end deep learning project, including the model training, evaluation, and CICD deployment. A key part of this is preparing the base model using transfer learning techniques. I freeze certain layers during training, save the model using MLflow, and create a prepare base model training pipeline with MLflow and DVC.


Finally, I build a Flask-based prediction application that can accept medical images, convert them to the appropriate format, and use the deployed deep learning model to detect the presence of chest cancer. Throughout the project, I emphasize the importance of using MLOps tools like MLflow and DVC for experiment tracking, model registration, pipeline tracking, and artifact management. These tools are essential for keeping my chest cancer detection deep learning project organized, reproducible, and scalable.