# my-first-app

# Setup

Create and activate a virtual environment:

```sh
conda create -n my-first-env python=3.10

conda activate my-first-env
```


Install packages:

```sh
pip install -r requirements.txt
```

Obtain an [API Key from Alphavantage](https://www.alphavantage.co/support/#api-key) or from the prof (`ALPHAVANTAGE_API_KEY`).



Create a ".env" file and paste in the following contents:

```sh
# this is the ".env" file...

ALPHAVANTAGE_API_KEY="_________"
MAILGUN_API_KEY="_______"
MAILGUN_SENDER_ADDRESS="________"
MAILGUN_DOMAIN="sandbox____.mailgun.org"
```

You must first follow the [setup instructions](https://github.com/prof-rossetti/intro-to-python/blob/main/notes/python/packages/sendgrid.md) to create an account, verify your account, setup a single sender, and obtain an API Key.

# Usage

Run the example script:

```sh
python app/my_script.py
```

Run the unemployment report:
```sh
#python app/unemployment.py
python -m app.unemployment
```

send an email:

```sh
python app/email_service.py
