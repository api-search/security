---
anonymous_access: false
api_key_in: []
api_specs:
- filename: open-government-new-south-wales-browse-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Browse API
  slug: open-government-new-south-wales-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-browse-api-openapi.yml
- filename: open-government-new-south-wales-details-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Details API
  slug: open-government-new-south-wales-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-details-api-openapi.yml
- filename: open-government-new-south-wales-fuelcheckrefdata-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Fuel Check Ref Data API
  slug: open-government-new-south-wales-fuelcheckrefdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-fuelcheckrefdata-api-openapi.yml
- filename: open-government-new-south-wales-fuelpricecheck-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Fuel Price Check API
  slug: open-government-new-south-wales-fuelpricecheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-fuelpricecheck-api-openapi.yml
- filename: open-government-new-south-wales-pharmacyregister-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Pharmacyregister API
  slug: open-government-new-south-wales-pharmacyregister-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-pharmacyregister-api-openapi.yml
- filename: open-government-new-south-wales-security-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Security API
  slug: open-government-new-south-wales-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-security-api-openapi.yml
- filename: open-government-new-south-wales-verify-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Verify API
  slug: open-government-new-south-wales-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-verify-api-openapi.yml
auth_types: []
description: API NSW generates API keys for APIs and enables authentication to your APIs using policies. Credential pairs consisting of consumer key and secret are provisioned to clients and stored for future validation. Apps must be approved by an api.nsw administrator before keys are usable.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Open Government New South Wales Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Government, New South Wales declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Open Government, New South Wales
provider_slug: open-government-new-south-wales
scheme_count: 2
schemes:
- credential_exchange: HTTP Basic header carrying base64 of "Key:Secret"
  flow: clientCredentials
  tokenUrl: https://api.onegov.nsw.gov.au/oauth/client_credential/accesstoken?grant_type=client_credentials
  token_lifetime_text: an authorisation token that would last approximately 12 hours from the time when request was made
  token_usage: Authorization Bearer header on every subsequent request
  type: oauth2
- description: API key sent alongside the bearer token on each data call (spec header parameter apikey)
  in: header
  name: apikey
  type: apiKey
slug: open-government-new-south-wales-authentication
source_filename: open-government-new-south-wales-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://api.nsw.gov.au/Product/Index/22\ndocs: https://api.nsw.gov.au/Support\nschemes:\n- type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://api.onegov.nsw.gov.au/oauth/client_credential/accesstoken?grant_type=client_credentials\n  credential_exchange: HTTP Basic header carrying base64 of \"Key:Secret\"\n  token_lifetime_text: an authorisation token that would last approximately 12 hours from the time when request was made\n  token_usage: Authorization Bearer header on every subsequent request\n- type: apiKey\n  in: header\n  name: apikey\n  description: API key sent alongside the bearer token on each data call (spec header parameter apikey)\ndescription: API NSW generates API keys for APIs and enables authentication to your APIs using policies. Credential pairs consisting of consumer key and secret are provisioned to clients and stored for future validation. Apps must be approved by an api.nsw administrator before\
  \ keys are usable.\nnote: The contract declares no securitySchemes; the token operation (OauthClientCredentialAccesstokenGet, GET /oauth/client_credential/accesstoken) and the Authorization/apikey header parameters are in openapi/open-government-new-south-wales-fuel-openapi.yml. Not probed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/authentication/open-government-new-south-wales-authentication.yml
summary_line: 2 schemes
tags:
- Government
- Public APIs
- Open Data
- Australia
- New South Wales
- Public Sector
- Fuel Prices
---
