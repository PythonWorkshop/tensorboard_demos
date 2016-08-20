# Make Sense of Deep Neural Networks using TensorBoard

## Getting Started

First, fetch the repo: [github.com/PythonWorkshop/tensorboard_demos](https://github.com/PythonWorkshop/tensorboard_demos)

```bash
git clone git@github.com:PythonWorkshop/tensorboard_demos
cd tensorboard_demos/
```

Then, choose one of the options below: conda (if you have [Anaconda](https://www.continuum.io/downloads) and [conda-env](https://github.com/conda/conda-env)) or pip.

_Note: Notebooks in this repo are written in Python 3. You'll also need Jupyter/iPython to run them._

### Option A: Conda install

1. Create a conda environment (auto-installs packages as per `environment.yml`) and activate it:

  ```bash
  conda env create
  source activate tensorflow
  ```

2. Run notebook:

  ```bash
  jupyter notebook tensorboard_basics.ipynb
  ```

_For troubleshooting, see TensorFlow's [conda install instructions](https://www.tensorflow.org/versions/master/get_started/os_setup.html#anaconda-installation)._

### Option B: Pip install

1. Install dependencies first (NumPy, matplotlib, scikit-learn):

  ```bash
  pip install numpy matplotlib scikit-learn
  ```

2. Install TensorFlow as per [instructions](https://www.tensorflow.org/versions/master/get_started/os_setup.html#pip-installation).

3. Run notebook:

  ```bash
  jupyter notebook tensorboard_basics.ipynb
  ```

## Binder (_coming soon_)

If you have trouble getting TensorFlow to work, go to the [repo](https://github.com/PythonWorkshop/tensorboard_demos) and hit the **launch binder** badge to run in the cloud. Note that this is experimental prone to failure.
