# File: README.md

# Kiambu Dairy Co-op Payment Calculator

A simple command-line tool that calculates how much a dairy farmer should be paid for the milk they deliver, based on the current buying price per litre.

## What It Does

- Reads the current buying price from a price.txt file(Price updated every Week)
- Falls back to a default price of KES 55.0 per litre if the price.txt file is missing
- Asks for inputs of the farmer(name, litres supplied)
- Validates inputs (name is required, litres must be integer, and greater than zero)
- Prints a clear payment summary

## Setup

```bash
pip install -r requirements.txt
```

## Usage

``` 
Run the program from the project's folder

python dairy_calculator_clt.py
```

## How It Works

Payment is calculated as the set price per litre is multiplied by the number of litres keyed in by the milk supplier
 
```python

def calculate_payment(litres, price_per_litre):
    return litres * price_per_litre

```

## Sample Output

```
Kiambu Dairy Co-op Payment Calculator
--------------------------------------
Current buying price: KES 55.00 per litre

Farmer name: Mwangi
Litres supplied today: 85

Farmer : Mwangi
Litres : 85.0
Price  : KES 55.00/litre
Total  : KES 4,675.00

```

## Stack

Python

