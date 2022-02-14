# Balance Novels

The Jupyter notebook in this repository describes and analyses the status quo of the [roman18 corpus](https://github.com/MiMoText/roman18) in the context of the ["Mining and Modeling Text"](https://www.mimotext.uni-trier.de/) project with respect to criteria such as author gender, year of first publication, narrative form etc. It then compares it to the "baseline" of the "Bibliographie du genre romanesque français, 1751-1800" (BGRF).

BGRF data sources: 
- Martin, Angus, Vivienne Mylne, und Richard L. Frautschi. Bibliographie du genre romanesque français, 1751-1800. London: Mansell, 1977.
- Lüschow, Andreas. Bibliographie du genre romanesque français, 1751-1800: RDF model [Data set]. French. Trier: Trier University, 2019. http://doi.org/10.5281/zenodo.3401428.

## Prerequisites

All the python dependencies are listed in `requirements.txt`. You can use `pip` or a similar tool to install them with

```
pip install -r requirements.txt
```

Part of the notebook uses data from our Wikibase instance. For this to work, currently you need to have access to the campus net of the University Trier. Everything else should be freely accessible.


## Usage

You can start the notebook as usual with

```
jupyter notebook balance_analysis.ipynb
```

Some of the more intricate utility functions have been outsourced into their own `utils.py` module. They can be modified there, the changes will get picked up on the next re-run of the notebook (i.e. when the notebook kernel is reloaded).


## Testing

For the utility functions that have been outsourced into their own `utils.py` module, unit tests are provided in `test/test_utils.py`. To run the test suite, simply execute the following (from the root folder of this repo):

```
python -m unittest discover
```

Failing test cases are regressions and should therefore be considered as bugs. 


## License

This software is available under the terms of the MIT license

