Data Parsing Firebase
=====================

Data Parsing Firebase is a Python script designed to parse data from an Excel sheet and upload it to a Firebase database. This project simplifies the process of integrating data from Excel sheets into Firebase, enabling efficient storage and retrieval.

Prerequisites
-------------

- Python 3.x installed on your system.
- A Firebase project created and configured.
- `firebase_admin` and `google.cloud` Python packages installed. You can install them using pip:

      pip install firebase_admin google-cloud

  
Getting Started
---------------

1. Clone this repository or download the `main.py` file to your local machine.

2. Place your Excel sheet (`*.csv` format) in the same directory as `main.py`.

3. Update the `file_path` variable in `main.py` to specify the name of your Excel sheet.

4. Make sure you have downloaded the service account key JSON file from your Firebase project settings and saved it in the same directory as `main.py`. Update the `Certificate` function call with the correct path to your JSON file.

5. Run the `main.py` script using the following command:

        python main.py


6. The script will parse the data from the Excel sheet, create a batch of Firestore documents, and upload them to your specified collection in Firebase.

Configuration
-------------

- `file_path`: Specify the path to your Excel sheet (CSV format).
- `collection_name`: Specify the name of the Firestore collection where you want to store the data.

Limitations
-----------

- The script currently assumes that the first row of the Excel sheet contains headers.

Contributors
------------

- Khushboo Shrivastava

License
-------

This project is licensed under the [MIT License](LICENSE).
