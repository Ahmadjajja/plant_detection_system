# Plant Disease Detection System

This repository contains the code for a Plant Disease Detection System, which uses deep learning techniques to identify and classify plant diseases from images. The system is built with a combination of Flask for the web application, TensorFlow and Keras for the model, and various other libraries for image processing and data visualization.

## Project Structure

- **.ipynb_checkpoints**: Contains checkpoints for Jupyter Notebook.
- **Dataset**: Folder containing images for training, testing, and validation.
- **static**: Folder for static files like CSS, JavaScript, and images.
- **templates**: Folder containing HTML templates (`index.html` and `import.html`).
- **uploads**: Folder where uploaded images are temporarily stored.
- **.gitignore**: File specifying which files and directories to ignore in Git.
- **app.py**: Main application file for the Flask web app.
- **Model_Training.ipynb**: Jupyter Notebook for training the plant disease detection model.
- **model.h5**: Pre-trained model file.
- **README.md**: This file.
- **requirement.txt**: File listing the required Python packages.

## Requirements

To run this project, the following Python packages are required:

- Flask
- numpy
- opencv-python
- Pillow
- tensorflow
- keras
- IPython
- scipy
- matplotlib
- seaborn

These can be installed using the following command:

```bash
pip install -r requirements.txt
```

# Model Training

The model is trained using the Model_Training.ipynb Jupyter Notebook. This notebook includes all the steps for preprocessing the data, building the model, training, and evaluating it. The dataset is divided into training, testing, and validation sets, which are used to ensure the model's accuracy and reliability.

# Web Application

The web application is built using Flask. The app.py file contains the code for the web server and handles routes and predictions.

## Main Files:
- **app.py**: Contains the Flask application code. It loads the pre-trained model (model.h5), processes incoming images, and returns predictions.
- **templates/index.html**: The main HTML file for uploading images and displaying results.

## Running the Application
To run the web application, execute the following command:

```bash
python app.py
```
Once the server is running, navigate to http://127.0.0.1:5000/ in your web browser to use the application.

Prediction Workflow
- **Upload an Image**: Use the web interface to upload an image of a plant leaf.
- **Process the Image**: The image is preprocessed and fed into the pre-trained model.
- **Get Results**: The model predicts the disease and displays the result on the web page.


# Dataset

The dataset contains images of plant leaves categorized into healthy and various diseased classes (e.g., Powdery mildew, Rust). These images are organized into three parts:

- **Train**: Images used for training the model.
- **Test**: Images used for testing the model.
- **Validation**: Images used for validating the model's performance.

# Contribution

Feel free to contribute to this project by opening issues or submitting pull requests. For major changes, please open an issue first to discuss what you would like to change.
