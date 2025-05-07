# WeatherShopper Automation

This project uses **Selenium with Python** to automate the shopping process on [WeatherShopper](https://weathershopper.pythonanywhere.com/), an e-commerce demo site for testing automation tools.

## Features

- Opens the moisturizer or sunscreen page
- Adds a product to the cart
- Navigates to the cart
- Clicks the **"Pay with Card"** button (Stripe integration)
- (Optional) Fills out the Stripe payment form (disabled in this version)

## Bug Found through Automation

When adding a product to the cart twice (or more), the **price of the product does not increase** as expected. This is a bug on the website where the price remains fixed even though multiple items are added to the cart. It may affect users who intend to purchase more than one unit of the same product.

##  Requirements

- Python 3.7+
- Google Chrome
- ChromeDriver (matching your browser version)
- Selenium

## Installation

1. **Clone this repository**:
    ```bash
    git clone https://github.com/your-username/weathershopper-automation.git
    cd weathershopper-automation
    ```

2. **Install dependencies**:
    ```bash
    pip install selenium
    ```

3. **Download ChromeDriver**:
    - Get the version matching your Chrome from: https://sites.google.com/chromium.org/driver/
    - Place it in your PATH or project folder.

## Usage

Run the automation script with:

```bash
python weathershopper_bot.py

