---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for the webphone token endpoint requires a Bulut Santral API key passed as a query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Verimor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verimor declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Verimor
provider_slug: verimor
scheme_count: 1
schemes:
- evidence: webphone_tokens isteği API anahtarı gerektirir — bu isteği tarayıcıdan doğrudan atmayın.
  how_to_obtain: Obtain the API key from the Bulut Santral portal and include it as the 'key' query parameter.
  location: query
  name: apiKey
  type: apiKey
slug: verimor-authentication
source_filename: verimor-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.verimor.com.tr/developer/recipes/webphone-oturumu-baslatma
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.verimor.com.tr/developer/recipes/webphone-oturumu-baslatma\nsources:\n- https://docs.verimor.com.tr/developer/recipes/webphone-oturumu-baslatma\ndescription: Authentication for the webphone token endpoint requires a Bulut Santral API key passed as a query parameter.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: webphone_tokens isteği API anahtarı gerektirir — bu isteği tarayıcıdan doğrudan atmayın.\n  location: query\n  how_to_obtain: Obtain the API key from the Bulut Santral portal and include it as the 'key' query parameter.\ndocs: https://docs.verimor.com.tr/developer/recipes/webphone-oturumu-baslatma\n"
source_yaml_url: https://artifacts.apis.io/verimor/authentication/verimor-authentication.yml
summary_line: 1 scheme
tags:
- SMS
- WhatsApp
- API
---
