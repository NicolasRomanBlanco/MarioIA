# MarioIA

## Requirements

- Visual studio build tools (In the installation, you'll need to click on the section labeled 'Desktop development with C++')

- CUDA Toolkit 11.8 (If you don't have a graphics card or want to use the CPU (not recommended), you should download PyTorch accordingly. To download your version, go to https://pytorch.org)

- If you encounter problems while trying to install stable-baselines3, run 'pip install --upgrade pip wheel==0.38.4 setuptools==65.5.1'


## How to use

The first cell only needs to be executed once; then run the cells one by one until you reach the one where the model is trained. I recommend training for at least 1 million timesteps to see results, although it surpassed the first level at 4 million. To test it, you'll need to execute the next cell and change './train/best_model_XXXXX', where XXXXX is the number of the model you want to test that has been saved in the 'train' folder

## Logs

To see the logs, you need to open a terminal (I use Git Bash) in the folder where you have the environment. Navigate to where you have the logs. In my case, it would be something like 'PythonVenv\jupyter_playground\Projects\Mario\logs'. You'll see a folder named PPO_X, where X represents the training number. Enter this folder and run the following command: 'tensorboard --logdir=.'
