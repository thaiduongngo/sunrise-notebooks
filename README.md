# Installation
## Setup Environment
You can use either virtual environment from Python or Conda framework
### Opt1: Virtual Environment
#### Install Python
https://www.python.org/downloads/
(Recommended Python 3.12.7)
### Create virtual environment
```
python3 -m venv .venv
```
#### Activate virtual environment
*MacOS:* ```source .venv/bin/activate```
#### Install Libraries
```
pip install pip -U
```
```
pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow torch imblearn jupyter -U
```
### Opt2: Conda
#### Install Miniconda
https://docs.anaconda.com/miniconda/
#### Create environment
```
conda create --name sunrise-notebooks python=3.12.7 pip
```
where sunrise-notebooks is the name of environment
#### Activate Environment
```
conda activate sunrise-notebooks
```
#### Install Libraries
```
pip install pip -U
```
```
conda config --append channels conda-forge
```
```
conda install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow jupyter
```
```
conda install pytorch::pytorch -c pytorch
```
```
pip install imblearn  -U 
```
Only applicable for MacOS ARM
```
conda install "libblas=*=*accelerate"
```
### Run Jupyter Notebook
```
jupyter notebook
```
# Basic Concepts
- **TP**: True Positive
- **TN**: True Negative
- **FP**: False Positive
- **FN**: False Negative

$$ Accuracy = \frac{TP + TN}{TP + TN + FP + FN} $$

$$ Precision = \frac{TP}{TP + FP} $$

$$ Recall = \frac{TP}{TP + FN} $$

$$ f1 = 2(\frac{Precision * Recall}{Precision + Recall}) $$

# Linear Regression

$$ f(x) = f_{(w,b)}(x) = wx + b $$

*w, b: parameters, coefficients*

## Cost function
*Squared error cost function*

$$ J_{(w,b)} = \frac{1}{2m}\sum\limits_{i=1}^{m} (\hat{y}^{(i)} - y^{(i)})^2 $$

# Entropy
Entropy: Suprise factor/indicator denoted **E**
## Formula
$$ E = \sum p(x) log(\frac{1}{p(x)}) $$

For example:

A set A consists 7 black balls and 1 red ball.

**p(black)** = 7/8 = 0.875 <br/>
**p(red)** = 1/8 = 0.125 <br/>
**S(black)** = log<sub>2</sub>(1/0.875) = 0.1926 <br/>
**S(red)** = log<sub>2</sub>(1/0.125) = 3

**E** = 0.875 * 0.1926 + 0.125 * 3 = 0.169 + 0.375 = **0.544**
