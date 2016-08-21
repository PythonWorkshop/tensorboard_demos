# Make Sense of Deep Neural Networks using TensorBoard

[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org:/repo/pythonworkshop/tensorboard_demos)

## Getting Started

_Note: Notebooks in this repo are written in Python 3. You'll need Jupyter/iPython to run them._

### Local installation

Fetch the repo: [github.com/PythonWorkshop/tensorboard_demos](https://github.com/PythonWorkshop/tensorboard_demos)

```bash
git clone git@github.com:PythonWorkshop/tensorboard_demos
cd tensorboard_demos/
```

Then, choose one of the options below: Conda (if you have [Anaconda](https://www.continuum.io/downloads) and [conda-env](https://github.com/conda/conda-env) installed), otherwise pip.

#### Option A: Conda install

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

#### Option B: Pip install

1. Install dependencies first (NumPy, matplotlib, scikit-learn):

  ```bash
  pip3 install numpy matplotlib scikit-learn
  ```

2. Install TensorFlow as per [instructions](https://www.tensorflow.org/versions/master/get_started/os_setup.html#pip-installation).

3. Run notebook:

  ```bash
  jupyter notebook tensorboard_basics.ipynb
  ```

### Binder

[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org:/repo/pythonworkshop/tensorboard_demos)

If you have trouble getting TensorFlow to work, hit the **launch binder** badge to run in the cloud. Note that this is an experimental feature.

## Running TensorBoard

Follow the notebook to build a neural network and train it. During training, make sure events are logged using [`tf.train.SummaryWriter`](https://www.tensorflow.org/versions/r0.10/api_docs/python/train.html#SummaryWriter) (code included in demo). Then run TensorBoard, pointing it to the log directory:

```bash
tensorboard --logdir=logs
```

And then open the URL that gets printed, in your browser (typically: [http://0.0.0.0:6006](http://0.0.0.0:6006)).

Explore the structure of the neural network in the Graph tab, and the summaries you reported in the Events tab.
