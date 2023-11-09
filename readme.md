
## Introduction

Welcome to our project! This notebook was run in Kaggle, and if you want to run it locally, there are a few changes you'll need to make. 

## Local Setup

1. **Dependencies:**
   Make sure you have all the dependencies installed. You can find the list in the `requirements.txt` file.

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
   - GSV Cities dataset: [Link to Dataset](your_gsv_cities_dataset_link)
   - Mapillary Cities dataset: [Link to Dataset](your_mapillary_cities_dataset_link)

   Make sure to place the datasets in the appropriate directories or update the paths in the code accordingly.

5. **Scheduler:**
   Uncomment and use the scheduler that is required for your experiment. If using the original scheduler, skip this step. 

## Running the Code

Once you've completed the setup, you can run the notebook locally. Make sure to follow the instructions in the notebook for any additional configuration or steps.

Happy experimenting!
