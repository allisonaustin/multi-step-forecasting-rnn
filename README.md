# multi-step-forecasting-rnn

This project contains an implementation of a multi-step forecasting model using Recurrent Neural Networks (RNN).

## Running the project locally

1. Install required libraries/modules
   - pandas
   - numpy
   - tensorflow
   - sklearn
   - keras
   - random
   - matplotlib


1. Download or clone the repository 
2. Open MLProject.ipynb in your IDE
3. Run the following cell: 
   ```python
   import pandas as pd
   # loading the dataset locally (do not run this cell if using colab)
   day_ds = pd.read_csv('data/day.csv')
   hour_ds = pd.read_csv('data/hour.csv')
   ```
4. Skip the following cell:
   ```python
   from google.colab import drive
   drive.mount('/content/gdrive')
   day_ds = pd.read_csv('/content/drive/MyDrive/Colab Notebooks/day.csv')
   hour_ds = pd.read_csv('/content/drive/MyDrive/Colab Notebooks/hour.csv')
   ```


## Setting up the Project in Google Colab

To set up this project in Google Colab, follow these steps:

1. **Mount Google Drive in Colab**:
   Use the following code snippet to mount your Google Drive to the Colab environment. This will allow Colab to access and save files to your Google Drive.

    ```python
    from google.colab import drive
    drive.mount('/content/gdrive')
    ```

    After running this code, you'll need to follow the instructions to authorize Colab to access your Google Drive.

2. **Navigate to Your Project Directory**:
   Change the directory to where you want to clone the repository in your Google Drive.

    ```python
    %cd gdrive/MyDrive/path-to-project
    ```

    Adjust the path `path-to-project` to the location where you want the project to be cloned.

3. **Clone the Repository**:
   Execute the following command to clone the repository into the specified directory.

    ```python
    !git clone https://username:token@github.com/allisonaustin/multi-step-forecasting-rnn.git
    ```

    Replace `username:token` with your GitHub username and a personal access token. The token is necessary for authentication if you're cloning a private repository or if your GitHub account has two-factor authentication enabled.

