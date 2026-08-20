---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Takepayments Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: takepayments secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: takepayments
provider_slug: takepayments
scheme_count: 2
schemes:
- api: takepayments Terminal API
  api_hosts:
    production: https://takepayments-integrated-prod-apim.azure-api.net/
    sandbox: https://takepayments-integrated-sandbox-apim.azure-api.net/
  credentials:
  - client_id
  - client_secret
  - scope
  discovery:
  - well-known/takepayments-openid-configuration-prod.json
  - well-known/takepayments-openid-configuration-sandbox.json
  flow: clientCredentials
  identity_provider: Microsoft Azure AD / Azure AD B2C
  name: TerminalApiOAuth2
  request_header: 'Authorization: Bearer {JWT}'
  scope_format: https://takepaymentsintegratedprod.onmicrosoft.com/{ClientId}/.default
  sources:
  - https://developer.takepayments.com/documentation/authentication
  tenants:
    production: takepaymentsintegratedprod.onmicrosoft.com
    sandbox: takepaymentsintegrated.onmicrosoft.com
  token_endpoints:
    production: https://login.microsoftonline.com/0bdad8b5-fe48-4ccd-b807-e6b2662a6d0c/oauth2/v2.0/token
    sandbox: https://login.microsoftonline.com/cf77fc4a-626b-46ff-bd3a-3400a727352f/oauth2/v2.0/token
  type: oauth2
- api: takepayments Gateway API
  in: body
  mechanism: Merchant ID plus a pre-shared-key (PSK) signature hash computed over the request fields; sent inside the SOAP v1.1 XML / HTTPS form-POST message rather than an HTTP header.
  name: GatewayMerchantSignature
  sources:
  - https://www.takepayments.com/developer-support/
  type: apiKey
slug: takepayments-authentication
source_filename: takepayments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://developer.takepayments.com/documentation/authentication\nsummary:\n  types: [oauth2, apiKey]\n  oauth2_flows: [clientCredentials]\n  api_key_in: [header]\n  note: >-\n    Two distinct APIs with two distinct auth models. The modern Terminal API\n    uses OAuth 2.0 client-credentials issued by Microsoft Azure AD (JWT bearer).\n    The legacy online payment Gateway API authenticates each SOAP/form-POST\n    message with a merchant ID plus a pre-shared-key signature hash (not a\n    bearer token).\nschemes:\n- name: TerminalApiOAuth2\n  api: takepayments Terminal API\n  type: oauth2\n  flow: clientCredentials\n  identity_provider: Microsoft Azure AD / Azure AD B2C\n  token_endpoints:\n    production: https://login.microsoftonline.com/0bdad8b5-fe48-4ccd-b807-e6b2662a6d0c/oauth2/v2.0/token\n    sandbox: https://login.microsoftonline.com/cf77fc4a-626b-46ff-bd3a-3400a727352f/oauth2/v2.0/token\n  tenants:\n    production: takepaymentsintegratedprod.onmicrosoft.com\n\
  \    sandbox: takepaymentsintegrated.onmicrosoft.com\n  scope_format: 'https://takepaymentsintegratedprod.onmicrosoft.com/{ClientId}/.default'\n  credentials: [client_id, client_secret, scope]\n  request_header: 'Authorization: Bearer {JWT}'\n  api_hosts:\n    production: https://takepayments-integrated-prod-apim.azure-api.net/\n    sandbox: https://takepayments-integrated-sandbox-apim.azure-api.net/\n  discovery:\n  - well-known/takepayments-openid-configuration-prod.json\n  - well-known/takepayments-openid-configuration-sandbox.json\n  sources: [https://developer.takepayments.com/documentation/authentication]\n- name: GatewayMerchantSignature\n  api: takepayments Gateway API\n  type: apiKey\n  in: body\n  mechanism: >-\n    Merchant ID plus a pre-shared-key (PSK) signature hash computed over the\n    request fields; sent inside the SOAP v1.1 XML / HTTPS form-POST message\n    rather than an HTTP header.\n  sources: [https://www.takepayments.com/developer-support/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/takepayments/refs/heads/main/authentication/takepayments-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Card Payments
- Card Machines
- In-Person Payments
- E-Commerce
- PSP
- Acquiring
---
