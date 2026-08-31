---
api_key_in: []
auth_types: []
description: 'Every Proactis REST API is protected by two credentials used together on the same request: an OAuth 2.0 bearer access token obtained through the client credentials grant, and a fixed API key sent in the x-api-key header. Credentials are issued by Proactis support on request — there is no self-service client registration.'
kind: authentication
layout: security
method: searched
name: Proactis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proactis declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Proactis
provider_slug: proactis
scheme_count: 0
schemes: []
slug: proactis-authentication
source_filename: proactis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.proactis.com/using-the-api/authentication\nprovider: Proactis\nproviderId: proactis\nname: Proactis API authentication\ndescription: >-\n  Every Proactis REST API is protected by two credentials used together on the same\n  request: an OAuth 2.0 bearer access token obtained through the client credentials\n  grant, and a fixed API key sent in the x-api-key header. Credentials are issued by\n  Proactis support on request — there is no self-service client registration.\nnotes:\n  - >-\n    Both credentials are required. An OAuth token alone, or an API key alone, is\n    rejected — the docs state that requests missing or carrying an incorrect token or\n    API key return 401 Unauthorized.\n  - >-\n    There is no self-service developer signup. The docs say \"For initial registration\n    and to obtain OAuth 2.0 credentials, please contact Proactis support.\"\n  - All requests must be made over HTTPS; plain HTTP calls\
  \ fail.\nsecuritySchemes:\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      OAuth 2.0 client credentials grant (RFC 6749), server-to-server. The client posts\n      grant_type=client_credentials to the regional token endpoint with the client id and\n      client secret supplied as HTTP Basic credentials in the Authorization header and\n      Content-Type application/x-www-form-urlencoded.\n    tokenRequest:\n      method: POST\n      contentType: application/x-www-form-urlencoded\n      body: grant_type=client_credentials\n      clientAuthentication: basic\n      host: >-\n        Regional API host, e.g. apius.proactiscloud.com (US), apiuk.proactiscloud.com (UK),\n        regos2p-eu1-api.proactiscloud.com (EU), api.esize.nl (NL)\n    tokenResponse:\n      token_type: Bearer\n      expires_in: 3600\n      expires_in_unit: seconds\n    inHeader: 'Authorization: Bearer <access_token>'\n    identityProvider: >-\n      Amazon Cognito.\
  \ The published example token carries\n      iss https://cognito-idp.eu-west-2.amazonaws.com/<pool-id>, which places the\n      authorization server in AWS Cognito in the eu-west-2 (London) region.\n    scopes: see scopes/proactis-scopes.yml\n    docs: https://docs.proactis.com/using-the-api/authentication\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameterName: x-api-key\n    description: >-\n      A fixed API key issued alongside the OAuth client credentials at registration. Sent\n      on every API request in addition to the bearer token.\n    rotation: not documented\n    docs: https://docs.proactis.com/using-the-api/authentication\ntokenLifetime:\n  expires_in: 3600\n  renewal: >-\n    Access tokens have a limited validity period. On expiry the client repeats the client\n    credentials request with the same client id and secret. No refresh token is issued —\n    the client credentials grant does not use one.\noutboundAuthentication:\n  description: >-\n    Distinct\
  \ from inbound API auth: when Proactis PUSHES documents to a customer endpoint,\n    the customer chooses how Proactis authenticates to THEM. Configured per endpoint in\n    Communication Settings; zero, one or several types can be combined.\n  types:\n    - BASIC\n    - USERNAME_PASSWORD\n    - OAUTH2\n    - API_KEY\n  docs: https://docs.proactis.com/using-the-api/transactions/push-transactions\nselfService: false\nmtls: false\nopenIdConnect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proactis/refs/heads/main/authentication/proactis-authentication.yml
summary_line: 0 schemes
tags:
- Procurement
- Purchase-To-Pay
- Source-To-Pay
- Spend Management
- Contract Management
- eInvoicing
- Accounts Payable
- Supplier Management
- eSourcing
- cXML
- UBL
- SCIM
---
