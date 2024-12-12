# Vehicle Number Plate Detection and Classification

This project involves detecting number plates on vehicles, reading the text on the plates, classifying vehicles into predefined categories (e.g., car, truck, bus), and storing the processed data in a database. The project is designed to integrate seamlessly for both Kaggle and local environments.

## Features

- **Number Plate Detection**: Uses a YOLO-based model to detect vehicle number plates.
- **OCR for Text Recognition**: Extracts text from number plates using EasyOCR.
- **Vehicle Classification**: Classifies vehicles into categories such as car, truck, or bus.
- **Data Storage**: Records extracted information (number plate text, vehicle type) in a database for further analysis.
- **Integration for Local Use**: Combines detection and classification models for deployment on local machines.

---

## Installation

### Prerequisites

1. Python 3.8 or above
2. pip (Python package manager)
3. A compatible environment with GPU support (optional but recommended)

### Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/your-repository/vehicle-detection.git
   cd vehicle-detection
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the pre-trained models:
   - Place the YOLO model weights in the `models/` directory.
   - Ensure the OCR model is set up correctly (handled automatically by EasyOCR).

---

## Usage

### For Kaggle Environment

1. Open the `licence-plate-detection.ipynb` file in Kaggle.
2. Run the notebook to process the data and view outputs directly in the Kaggle environment.

### For Local Environment

1. Open the `integration of both the model for local.ipynb` file.
2. Adjust file paths and database connection settings as needed.
3. Run the notebook to process video inputs or images locally.

---

## Directory Structure

```
vehicle-detection/
├── licence-plate-detection.ipynb       # Kaggle-specific notebook
├── integration of both the model for local.ipynb  # Local integration notebook
├── models/                             # Pre-trained model weights
├── requirements.txt                    # Python dependencies
└── README.md                           # Project documentation
```

---

## Requirements

Refer to the `requirements.txt` file for a list of dependencies.

---

## Database Configuration

The project uses SQL with PyODBC for database interactions. To set up the database:

1. Install PyODBC:
   ```bash
   pip install pyodbc
   ```

2. Configure the database connection string in the notebook or script. Ensure you have the necessary permissions to connect to the database server.

3. Run the script or queries provided in the notebook to initialize the database schema.

---

## Models

- **YOLO**: For number plate detection
- **EasyOCR**: For reading text from detected number plates
- **Custom Classifier**: For vehicle classification (trained separately)

---

## Results

- Accurate detection and classification of vehicles.
- Reliable text extraction from number plates.
- Seamless integration of detection, classification, and database storage.

---


## Contributions

Feel free to submit issues or pull requests to improve this project.

---

## Contact

For any queries, contact Farhan at farhanfiaz79@gmail.com.
