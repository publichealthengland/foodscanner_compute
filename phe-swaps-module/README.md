# Recommender System for Public Health England

A recommender system which suggests healthier alternatives for each barcode scanned. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.


### Prerequisites

#### What things you need to install the software and how to install them:

- Access to PHE database to get live feed of products
- [Python 3.7](https://www.python.org/)/[Python (w/ Anaconda)](https://www.anaconda.com/)
- scipy>=1.4.1
- pandas==0.25.3
- numpy>=1.16.0
- scikit-learn>=0.22
- nltk>=3.4.5

### Installing

- From Source
Download the source code by cloning the repository or by pressing 'Download ZIP' on this page. Install by navigating to the package directory and running

```
python setup.py install
```

- Using Pip
You could install directly from Github:
'''
pip install https://github.com/Weber-Shandwick/phe_food_scanner 
'''

## Usage

```python
from phe_recommender.recommender import top_3_swaps, long_list_swaps, eligible_swaps, top_100_swaps

df = 'path to food_consolidated table'

eligible_swaps(barcode, df) # returns df of eligible swaps

long_list_swaps(barcode, df) # returns df of 30 top swaps

top_3_swaps(barcode, df) # returns df of top 3 swaps

top_100_swaps(barcode, df) # returns df of 100 swaps including top 3 swaps
```

### Exceptions 

Explain what these tests test and why

```
Give an example
```

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system


## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Daniele Dal Grande** - [ddalgrande](https://github.com/ddalgrande)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details