# Getting Started

Copy the project to a desired location:

    git clone https://github.com/sashawins/calculator-api.git
    cd calculator-api

# Usage

## Interacting with API:

`http://0.0.0.0:1337/` – **Main** – Shows the most recent calculation.  
`http://0.0.0.0:1337/recent` – **Recent** – Shows most recent 10 calculations.  
`http://0.0.0.0:1337/all` – **All** – Shows all calculations.  
`http://0.0.0.0:1337/operate?operation=x+y` – **Operate** – Operation performing template.

## Performing operation:

**Addition:**

    curl -X get http://0.0.0.0:1337/operate?operation=7%2b3

**Subtraction:**

    curl -X get http://0.0.0.0:1337/operate?operation=7-3

**Multiplication:**

    curl -X get http://0.0.0.0:1337/operate?operation=7*3

**Division:**

    curl -X get http://0.0.0.0:1337/operate?operation=7/3

# Deployment

    docker build -t calculator-api .
    docker run -p 1337:1337 calculator-api

# Reference

- [rohitamale18/calculator-api](https://github.com/rohitamale18/calculator-api)
