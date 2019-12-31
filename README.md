# fico-estimator

Fico-estimator is a Python =library for getting an aproximate fico score using a prescribed interest rate.
It is trained using 8,000 loans from Lending Clubs Marketplace. The library also includes a scraper for
collecting new loan data for further training and experimenting by adding other variables to the regression.

## Installation

Use the package manager [pip]

```bash
pip install fico-estimator
```

## Usage

```python
import fico-estimator as fe

#get a fico estimate
fe.predict_fico(rate)

#get lending club loan data from marketplace
fe.scrape(html)

#train using the new data. Returns regression intercept and coeficient (y = mx + b)
fe.train(data)
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
