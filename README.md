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
pip install pandas numpy matplotlib seaborn scikit-learn jupyter -U
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
