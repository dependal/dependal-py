[![PyPI](https://img.shields.io/pypi/v/dependal.svg)](https://pypi.org/project/dependal/)
[![Python Versions](https://img.shields.io/pypi/pyversions/dependal.svg)](https://pypi.org/project/dependal/)

# Dependal Python SDK

Official Python SDK for the **Dependal transactional email API**.

Dependal is a developer-first email delivery platform focused on
reliable transactional email, clear delivery logs, and predictable
pricing.

------------------------------------------------------------------------

## Installation

Install the SDK using pip:

``` bash
pip install dependal
```

------------------------------------------------------------------------

## Quick Start

``` python
from dependal import ApiClient, Configuration
from dependal.api.messages_api import MessagesApi

config = Configuration(
    host="https://api.dependal.com",
    api_key={"x-api-key": "dp-xxxxxxxxx"}
)

with ApiClient(config) as client:
    api = MessagesApi(client)

    api.send_email({
        "to": "user@example.com",
        "from": "Dependal <noreply@dependal.com>",
        "subject": "Hello",
        "html": "<p>This email was sent using Dependal.</p>"
    })
```

------------------------------------------------------------------------

## Documentation

Full documentation is available at:

https://dependal.com/docs

------------------------------------------------------------------------

## Features

-   Simple transactional email API\
-   Reliable delivery through Amazon SES\
-   Detailed email logs and event tracking\
-   Suppression handling\
-   Predictable developer-friendly pricing

------------------------------------------------------------------------

## Support

If you need help, contact:

support@dependal.com

------------------------------------------------------------------------

Built by **Dependal**.
