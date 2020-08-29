This repository demonstrates how to integrate [GitHub Actions](https://docs.github.com/en/actions) to (upon a new commit):

- Automatically authenticate `wandb` (Weights and Biases) using a custom GitHub secret. 
- Automatically train a small Random Forest Regressor model on the [wine quality dataset](https://www.kaggle.com/uciml/red-wine-quality-cortez-et-al-2009).
- Automatically log the training and other important model metrics to `wandb`. 
- Cache Python dependencies so that old dependencies do not get installed each time a run is triggered. 
- Generate a `metrics.csv` file after a run is successfully completed. 

<div align="center"><img src="https://i.ibb.co/JqZWHDC/image.png"></img></div>

The heart of this repository is [this YAML](https://github.com/sayakpaul/wine/blob/experiment-1/.github/workflows/cml.yaml) file that defines a workflow that runs automatically after a new commit is pushed. 

## Acknowledgments

[This video](https://www.youtube.com/watch?v=9BgIDqAzfuA) by DVCorg helped me a lot to clear the initial concepts regarding GitHub Actions. 
