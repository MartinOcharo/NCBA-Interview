
# Automation Engineer Coding Exercise
[![NCBA_LOOP](https://i.ibb.co/6rHQvxq/images.png)](https://ibb.co/Q8PWxQz)   [![Selenium](https://i.ibb.co/JxzY2tK/Screenshot-2024-08-29-at-02-02-15-Selenium-4.png)](https://ibb.co/Q8PWxQz)

This project is a solution to the Automation Engineer coding exercise provided by LOOP Digital Financial Services, the Digital Division of NCBA Bank. The task involves automating several steps using Selenium with any programming language, in my case Python. The tasks includes; account creation on Google and later logging in Jumia with the created Google account, product search, adding the product to the cart, navigating to it and  then generating a summary status report.

## Prerequisites

```bash
- Python 3.x
- Google Chrome browser
- ChromeDriver installed and added to your PATH
- Allure command-line tool installed - Installation Guide:) https://allurereport.org/docs/install/
```

## Installation

Install Dependencies:  

pip install these packages;

```bash
Selenium
Allure-pytest
Pytest
```

## Usage

```
1. pip install -r requirements.txt or run Main.py Sript.

2. Run the Test:
pytest tests/test_automation_flow.py --alluredir=reports/allure_results

3. View the Allure Report:
allure serve reports/allure_results

```

## Test Flow

The test performs the following steps:
1. Create a Google account: Automates the signup process on Google.
2. Create a Jumia account: Uses the Google account email to sign up on Jumia.
3. Search for the product: Searches for the product ?ailyons hd-199a electric dry iron box silver & black (1 yr wrty)? on Jumia.
4. Add the product to the cart: Adds the found product to the shopping cart.
5. Navigate to the cart: Verifies that the product has been added by navigating to the cart.


## Customization

- Browser Configuration: The default browser used is Chrome. If you wish to use a different browser, update the webdriver.Chrome() in conftest.py to the desired WebDriver.
- Test Data: Update the test data like email and password in the test_automation_flow.py or use a configuration file to manage test data.

## Troubleshooting

- ChromeDriver Issues: Ensure that ChromeDriver is compatible with your Chrome browser version.
- Email Sending Issues: Check your email credentials and ensure that your Gmail settings allow less secure apps or use an App Password if 2FA is enabled.

## Contact

For any questions or issues, feel free to reach out:

Email: martinocharoo@gmail.com

Phone: +254701684150

## Acknowledgments

1. https://github.com/Sakif1997/shopping-cart-automation?tab=readme-ov-file

2. https://pypi.org/project/selenium/

## Open- Source License

[Apache License Version 2.0](http://www.apache.org/licenses/)


