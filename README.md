# Eve Azure AD Auth

[![PyPI version](https://badge.fury.io/py/Eve-Azure-Auth.svg)](https://badge.fury.io/py/Eve-Azure-Auth)
[![Downloads](https://pepy.tech/badge/eve-azure-auth)](https://pepy.tech/project/eve-azure-auth)
[![Build Status](https://travis-ci.com/ateliedocodigo/eve-azure-auth.svg?branch=develop)](https://travis-ci.com/ateliedocodigo/eve-azure-auth)
![lint workflow](https://github.com/ateliedocodigo/eve-azure-auth/actions/workflows/lint.yml/badge.svg)
![test workflow](https://github.com/ateliedocodigo/eve-azure-auth/actions/workflows/test.yml/badge.svg)
[![Requirements Status](https://requires.io/github/ateliedocodigo/eve-azure-auth/requirements.svg?branch=develop)](https://requires.io/github/ateliedocodigo/eve-azure-auth/requirements/?branch=develop)


> Under development, it only validate token. Pull requests are welcome

## Read more

https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-protocols-oidc

## Usage

```bash
pip install Eve-Azure-Auth
```

## Setting up configuration

```python
AZURE_AD_TENANT = 'common'  # optional
AZURE_AD_ISSUER = 'https://login.microsoftonline.com/...'
AZURE_AD_AUDIENCES = 'id' # or ['id', 'id']
```

## Initialization

```python
from eve_azure_auth import AzureAuth

app = Eve(auth=AzureAuth)
```

*Voilà!*
