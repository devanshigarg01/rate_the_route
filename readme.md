
## Introduction

Welcome to our project! This notebook was run in Kaggle, and if you want to run it locally, there are a few changes you'll need to make. 

## Local Setup

1. **Dependencies:**
   Make sure you have all the dependencies installed. You can find the list in the `requirements.txt` file from [MixVpr](https://github.com/amaralibey/MixVPR/tree/main)

2. **Environment:**
   Set up a virtual environment to avoid conflicts with other projects.

   ```bash
   virtualenv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

   Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. **Experiment Tracking:**
   For experiment tracking, you need to add your WandB API key to Kaggle secrets or directly in the code. If using Kaggle secrets, make sure to update the code accordingly.

   ```python
   import wandb
   wandb.login(key="your-api-key")
   ```

4. **Dataset Download:**
   Download the necessary datasets:
   - GSV Cities dataset: [Link to Dataset](https://www.kaggle.com/datasets/amaralibey/gsv-cities) 
   - Mapillary Cities dataset: [Link to Dataset](https://www.mapillary.com/dataset/places)

   Make sure to place the datasets in the appropriate directories or update the paths in the code accordingly.

5. **Scheduler:**
   Uncomment and use the scheduler that is required for your experiment. If using the original scheduler, skip this step.


6. **GSV Cities Dataset Path:**
   Change the path where the GSV Cities dataset is stored in the code. Update the relevant variable to point to the correct directory.


7. **Pittsburg Dataset Path:**
   Change the path where the Pittsburgh dataset is cloned. Update the relevant variable to point to the correct directory.


8. **Train Cities List:**
   Add or remove cities from the train cities list based on your preference. Update the following list in the code:

   ```python
   train_cities = ['Bangkok', 'BuenosAires', 'LosAngeles', 'MexicoCity', 'OSL', 'Rome', 'Barcelona', 'Chicago', 'Madrid', 'Miami', 'Phoenix', 'TRT', 'Boston', 'Lisbon', 'Medellin', 'Minneapolis', 'PRG', 'WashingtonDC', 'Brussels', 'London', 'Melbourne', 'Osaka', 'PRS']
   ```

## Customization

9. **WandB Run Name:**
   Change the run name when initializing WandB. Update the following line with your preferred run name:

   ```python
   wandb.init(project="your_project_name", name="your_run_name")
   ```

10. **Number of Epochs:**
   Adjust the number of epochs in the trainer according to your experiment requirements. Update the following variable in the code:

   ```python
   num_epochs = your_preferred_number
   ```

## Running the Code

After making these changes, you can run the notebook locally. Follow the instructions in the notebook for any additional configuration or steps.
