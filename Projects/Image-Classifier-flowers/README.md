 # Image Classification with PyTorch


## Prerequisites
The Code is written in Python 3.6.5 . If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. 

To install pip run in the command Line
```
python -m ensurepip -- default-pip 
``` 
to upgrade it
```
python -m pip install -- upgrade pip setuptools wheel
```
to upgrade Python
```
pip install python -- upgrade
```
Additional Packages that are required are: [Numpy](http://www.numpy.org/), [Pandas](https://pandas.pydata.org/), [MatplotLib](https://matplotlib.org/), [Pytorch](https://pytorch.org/), PIL and json.\
You can donwload them using [pip](https://pypi.org/project/pip/)
```
pip install numpy pandas matplotlib pil
```
or [conda](https://anaconda.org/anaconda/python)
```
conda install numpy pandas matplotlib pil
```
In order to install PyTorch head over to the PyTorch site select your specs and follow the instructions given.	

### Project assets:

- `Image Classifier Project.ipynb` Jupyter Notebook
- `setup.py` Main Script
- `train.py` Command line tool to train a new network on a data set.
- `predict.py` Command line tool to to predict flower name from an image.


## Example Image for Training

Image categories are found in [cat_to_name.json]() and  flower images you can get in this repository itself or can be downloaded in the gziped tar file [flower_data.tar.gz](https://s3.amazonaws.com/content.udacity-data.com/nd089/flower_data.tar.gz) from Udacity.

Get flower images:
```bash
mkdir -p flowers && cd flowers
curl https://s3.amazonaws.com/content.udacity-data.com/nd089/flower_data.tar.gz | tar xz
```

You should now have **test**, **train** and **valid** directories containing classification directories and flower images under the **flowers** directory.

