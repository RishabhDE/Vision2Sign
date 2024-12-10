# Vision2Sign

Vision2Sign is a web application that uses a deep learning model to recognize American Sign Language (ASL) gestures from images. The application allows users to capture images using their webcam or upload images for prediction.

## Project Structure

- `ASL_EfficientNetB0_model.pth`: Pre-trained model weights for ASL recognition.
- `LICENSE`: License file for the project.
- `README.md`: This file.
- `Team03_Final_Project.ipynb`: Jupyter notebook containing the final project code and analysis.
- `Team03_Presentation-Slides.pptx`: Presentation slides for the project.
- `UI/`: Directory containing the web application code.
  - `app.py`: Flask application code.
  - `model/`: Directory containing the model weights.
    - `efficientnet_model.pth`: Model weights for EfficientNet.
  - `templates/`: Directory containing HTML and CSS files.
    - `index.html`: Main HTML file for the web application.
    - `styles.css`: CSS file for styling the web application.

## Setup and Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/RishabhDE/Vision2Sign
    cd Vision2Sign/UI
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Download the pre-trained model weights and place them in the `model/` directory.

## Running the Application

1. Start the Flask application:
    ```sh
    python app.py
    ```

2. Open your web browser and navigate to `http://localhost:5000`.

## Usage

- **Capture Image from Webcam**: Click the "Capture from Camera" button to capture an image using your webcam.
- **Upload Image**: Use the file input to upload an image from your device.
- The application will display the predicted ASL gesture along with the corresponding label.

## Model

The application uses an EfficientNet model pre-trained on ImageNet and fine-tuned for ASL recognition. The model is loaded and used for prediction in the `app.py` file.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- The EfficientNet model is provided by the `efficientnet_pytorch` library.
- The project uses Flask for the web application and PyTorch for the deep learning model.

## Contact

For any questions or inquiries, please contact the project team.
