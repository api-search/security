---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for delivery carrier integrations on meni.ge
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Meni Ge Authentication
name_suffix: Authentication
oauth_flows: []
overview: meni-ge declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: meni-ge
provider_slug: meni-ge
scheme_count: 3
schemes:
- evidence: 'Copy two values: Account (client ID) and Secure password (secret).'
  how_to_obtain: Create an API key in the CDEK account integration section and copy the Account (client ID) and Secure password (secret).
  name: CDEK API credentials
  type: apiKey
- evidence: Ask your manager for an online-store integration API key .
  how_to_obtain: Submit a connection request on fivepost.ru, sign the contract, and request the API key from the manager.
  name: 5Post API key
  type: apiKey
- evidence: Log in to my.novapost.com . Open “Integrations → API keys” and create a key. Copy the key.
  how_to_obtain: Log in to the My Nova Post account, go to Integrations → API keys, and create a new key.
  name: Nova Poshta API key
  type: apiKey
slug: meni-ge-authentication
source_filename: meni-ge-authentication.yml
source_heading: Authentication Profile
source_url: https://meni.ge/en/docs/delivery-cdek
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://meni.ge/en/docs/delivery-cdek\nsources:\n- https://meni.ge/en/docs/delivery-cdek\n- https://meni.ge/en/docs/delivery-yandex\n- https://meni.ge/en/docs/delivery-fivepost\n- https://meni.ge/en/docs/delivery-novaposhta\ndescription: Authentication methods for delivery carrier integrations on meni.ge\nschemes:\n- type: apiKey\n  name: CDEK API credentials\n  evidence: 'Copy two values: Account (client ID) and Secure password (secret).'\n  how_to_obtain: Create an API key in the CDEK account integration section and copy the Account (client ID) and Secure password (secret).\n- type: apiKey\n  name: 5Post API key\n  evidence: Ask your manager for an online-store integration API key .\n  how_to_obtain: Submit a connection request on fivepost.ru, sign the contract, and request the API key from the manager.\n- type: apiKey\n  name: Nova Poshta API key\n  evidence: Log in to my.novapost.com\
  \ . Open “Integrations → API keys” and create a key. Copy the key.\n  how_to_obtain: Log in to the My Nova Post account, go to Integrations → API keys, and create a new key.\ndocs: https://meni.ge/en/docs/delivery-cdek\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/meni-ge/authentication/meni-ge-authentication.yml
summary_line: 3 schemes
tags:
- Company
- POS
- Inventory
- CRM
- Hospitality
- E-commerce
---
