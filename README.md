## Keras + Tensorflow tutorials on Floyd

The Keras tutorials by [leriomaggio](https://github.com/leriomaggio/deep-learning-keras-tensorflow) 
is a great place to start learning Keras. It comes with structured Jupyter notebooks teaching Keras basics 
all the way to advanced concepts.

You can start by cloning the project repository and initializing a floyd project.

```bash
git clone https://github.com/leriomaggio/deep-learning-keras-tensorflow
cd deep-learning-keras-tensorflow
floyd init deep-learning-keras-tensorflow
```

If you don't have floyd already installed, you can run:
```bash
pip install -U floyd-cli
```

### GPU Mode

You can run this project on a GPU instance on Floyd with a single command:

```bash
floyd run --env keras --gpu --mode jupyter
```

The output should contain the url to the jupyter notebook:
```bash
Path to jupyter notebook: https://www.floydhub.com:8000/2sN82HNJhwsqUm5QbWtqUi
```

You can now open the Jupyter notebook url in your browser and start running the notebooks.

### Other Options

If you want to run this on a CPU instance:

```bash
floyd run --env keras --mode jupyter
```

And if you want a Python 2 environment, you can change it in the command line:

```bash
floyd run --env keras:py2 --gpu --mode jupyter
```

The full list of supported enviroments is [here](http://docs.floydhub.com/home/environments/).
