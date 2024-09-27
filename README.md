
![header](https://capsule-render.vercel.app/api?type=venom&height=300&color=gradient&customColorList=0,2,2,5,4,6,8,10,12,14,16,20,30&text=Stripe%20Key%20Validation&fontSize=75&animation=twinkling)
# Stripe Key Validation Script

This Node.js script checks both the **Publishable** and **Secret** keys for Stripe. It validates the format of the publishable key and verifies the secret key by making an API call to Stripe. If either key is invalid, it will display an error message.

## Features
- Validates if the publishable key starts with `pk_`.
- Attempts a test API call to Stripe with the secret key to verify its validity.
- Displays an error message if either key is invalid.
- Prints a success message if both keys are valid.

## Prerequisites

Before running the script, make sure you have the following prerequisites installed:

1. **Node.js**: Node.js is required to run the script. You can download and install it by following these steps:
   - Visit the [Node.js website](https://nodejs.org/en/).
   - Download the latest LTS (Long-Term Support) version for your operating system.
   - Follow the installation instructions for your platform (Windows, macOS, or Linux).
   
   After installation, you can verify if Node.js is installed correctly by running:
   
   ```bash
   node -v
   ```
# Stripe Account

You need a Stripe account to generate the publishable and secret keys.  
Go to the Stripe dashboard and create an account if you don't have one.  
Navigate to **Developers > API keys** in the Stripe dashboard to get your secret and publishable keys.  
Your secret key will start with `sk_` and your publishable key will start with `pk_`. Use the test keys for development purposes.

## Requirements

- Node.js (Installed as shown above)
- Stripe Secret and Publishable keys from your Stripe account

## Install the Stripe Package
```bash
npm install stripe
```
## Run The Code
```bash
node stripe-api-checker.js
```

