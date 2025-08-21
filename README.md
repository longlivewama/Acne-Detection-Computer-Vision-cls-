# Acne Detection Computer Vision Model

## Overview

This project is a deep learning-based classification model trained to identify and categorize different types of skin conditions related to acne. The model uses YOLO (You Only Look Once) for object detection and classification, and it is deployed as a web application using Streamlit. It can classify images into 16 distinct classes:

- Acne
- Blackhead
- Conglobata
- Crystanlline
- Cystic
- Flat_wart
- Folliculitis
- Keloid
- Milium
- Papular
- Purulent
- Scars
- Sebo-crystan-conglo
- Syringoma
- Unlabeled
- Whitehead

The application allows users to upload skin images for analysis, providing fast, reliable, and easy-to-interpret results to assist dermatologists and individuals in making informed decisions about skin health.

**Disclaimer:** This tool is for informational purposes only and is not a substitute for professional medical advice.

## Dataset

The model was trained on the Acne Detection dataset available at:  
[https://universe.roboflow.com/bangkit-academy-rnfpg/acne-detection-g5vvz](https://universe.roboflow.com/bangkit-academy-rnfpg/acne-detection-g5vvz)

## Features

- AI-powered dermatology assistant using advanced computer vision techniques.
- Supports classification of 16 types of acne and related skin conditions.
- User-friendly Streamlit interface for uploading and analyzing images.
- Displays prediction results with confidence scores and a progress bar.
- Includes a responsive UI with loading spinner and styled result cards.

## Requirements

To run this project, install the dependencies listed in `requirements.txt`. The project also requires the pre-trained model file `best.pt`, which should be placed in the project directory or specified with the full path in the code.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/acne-detection-model.git
   cd acne-detection-model
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Download the pre-trained model `best.pt` and place it in the appropriate directory (e.g., update the path in the Streamlit script if needed).

## Usage

1. Run the Streamlit application:
   ```
   streamlit run streamlit_app_update_st(final).py
   ```
   (Alternatively, use `acne_app.py` for a simpler version of the application.)

2. Open the app in your browser (typically at `http://localhost:8501`).

3. Upload a skin image (JPG, PNG, or JPEG format).

4. The app will analyze the image and display the predicted acne type along with a confidence score.

## Project Structure

- `streamlit_app_update_st(final).py`: Main Streamlit application with enhanced UI (progress bar, spinner, styled cards).
- `acne_app.py`: Simpler version of the Streamlit application.
- `app_run.txt`: Notes on running the app and dataset link.
- `best.pt`: Pre-trained YOLO model (not included; download separately).
- `README.md`: This file.
- `requirements.txt`: List of Python dependencies.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests for improvements, bug fixes, or new features.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details. (Note: Add a LICENSE file if needed.)