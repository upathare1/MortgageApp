# Mortgage Comparison Calculator

This project is a work-in-progress calculator for comparing the economic return of buying a home against renting and investing in stocks.

## Current Scope

The application models:

* Mortgage amortization, home appreciation, ownership costs, and tax deductions
* Rent growth and stock investing from available cash-flow differences
* After-tax liquidation values and Economic IRR
* Optional fixed monthly budgets for comparing financing strategies
* JSON scenario import and export

Financial calculations run server-side.

## Running the Application

### Build the Docker image

```bash
docker build -t mortgage-app .
```

### Run the container

```bash
docker run -p 3001:3000 mortgage-app
```

The application will then be available at:

```text
http://localhost:3001
```

## Status

This project is still under active development and assumptions, calculations, and features may change frequently.

## Disclaimer

This calculator provides estimates for informational purposes only. Results are not guaranteed to be accurate or complete and should not be relied upon as tax, legal, or financial advice. Please consult a qualified professional before making financial decisions.
