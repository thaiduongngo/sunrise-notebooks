# Installation
## Setup Environment
```
python3 -m venv .venv
```
## Activate virtual environment
**MacOS:** ```source .venv/bin/activate```
## Install Libraries
```
pip install pip -U
```
```
pip install jupyter pandas numpy matplotlib scikit-learn -U
```
Run Jupyter Notebook
```
jupyter notebook
```
# Linear Regression
$$ f(x) = f_{(w,b)}(x) = wx + b $$
*w, b: parameters, coefficients*

## Cost function
*Squared error cost function*
$$ J_{(w,b)} = \frac{1}{2m}\sum\limits_{i=1}^{m} (\hat{y}^{(i)} - y^{(i)})^2$$
