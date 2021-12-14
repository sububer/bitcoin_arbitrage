# Fintech Challenge 03 -- Bitcoin Arbitrage Analysis

An [analysis](#analysis) of bitcoin market prices across two exchanges, looking for arbitrage opportunities, using [pandas](https://pandas.pydata.org/).

---

## Analysis 

#### DataSets
Bitcoin market prices from two exchanges, with prices from Jan 1 2018 -> March 31 2018:
- [Bitstamp](./Resources/bitstamp.csv)
- [Coinbase](./Resources/coinbase.csv)

#### Assumptions
Three dates were chosen across the quarter from Jan -> March 2018: one early, middle and late in the quarter. Arbitrage opportunities were looked for from the Coinbase exchange to the Bitstamp exchange at each date.

#### Summary
There were significantly larger arbitrage opportunities at the beginning of the quarter than and the end, with the profitable spread actually at zero for the late quarter date. 

|Period | Cumulative Profit ($) |
| :---	| ---: |
|Early - Jan 16 2018 | 14147.17 |
|Middle- Feb 24 2018 | 330.07 |
|Late- Mar 26, 2018 | 0 |

See details and visualizations in the [notebook file](./crypto_arbitrage.ipynb)

---

## Technologies

This challenge uses [python](https://www.python.org/) 3.7 and the following [built-in](https://docs.python.org/3/py-modindex.html) modules:
- [pathlib](https://docs.python.org/3/library/pathlib.html#module-pathlib)

Additionally, it requires:
- [matplotlib](https://matplotlib.org/)
- [pandas](https://pandas.pydata.org/)
- [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/)

See [installation](#installation) below for specifics.

---

## Installation

You will need Python 3.7, that supports for this application to run. An easy way to install python 3.7 is to download and install [Anaconda](https://www.anaconda.com/products/individual). After installing anaconda, open a terminal/command-prompt, and setup a python 3.7 environment, and then activate it like so:

```
# create an anaconda python 3.7 environment
# name can be any friendly name to refer to your environment, eg 'dev'
conda create --name dev python=3.7 anaconda

# activating the environment
conda activate dev
```

---

## Usage

The analysis is presented within a [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) notebook. To launch JupyterLab, from the root of this repo dirctory:

```
# within repo root 
$ jupyter lab
```
You can now open the notebook [crypto_arbitrage.ipynb](./crypto_arbitrage.ipynb) locally with JupyterLab.

---

## Contributors

[David Lopez](https://github.com/sububer)

---

## License

MIT