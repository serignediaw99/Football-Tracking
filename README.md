# Football Tracking

This project uses YOLOv8 and Roboflow to train a model for tracking football players, referees, goalkeepers, and ball.

## Features

- Object detection and tracking for football players, referees, goalkeepers, and the ball
- Training pipeline using YOLOv8 and Roboflow
- Easy deployment and inference on new videos

## Prerequisites

- Python 3.8+
- Google Colab with GPU support (for training)
- Roboflow account

## Setup

1. Clone this repository:
   ```
   git clone https://github.com/serignediaw99/Football-Tracking.git
   cd Football-Tracking
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Set up your Roboflow account and create a `config.json` file in the `drive/MyDrive/` directory with the following structure:
   ```json
   {
     "roboflow_api_key": "your_roboflow_api_key",
     "workspace": "your_workspace_name",
     "project": "your_project_name",
     "version": "your_project_version"
   }
   ```

## Usage

1. Open the `train_model.ipynb` notebook in Google Colab or Jupyter Notebook.

2. Run the cells in order to:
   - Set up the environment
   - Prepare the dataset
   - Train the YOLOv8 model
   - Validate the model
   - Deploy the model to Roboflow

3. After training, you can use the `run_detections.ipynb` notebook to perform detections on new videos.

## Files

- `train_model.ipynb`: Notebook for training the YOLOv8 model
- `run_detections.ipynb`: Notebook for running detections on videos
- `requirements.txt`: List of required Python packages

## Acknowledgments

- [YOLOv8](https://github.com/ultralytics/ultralytics) for the object detection model
- [Roboflow](https://roboflow.com/) for dataset management and model deployment
- [Piotr Skalski](https://github.com/SkalskiP) for tutorial on how to train a YOLOv8 model for football tracking