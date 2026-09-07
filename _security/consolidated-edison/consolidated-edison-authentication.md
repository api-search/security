---
anonymous_access: false
api_key_in: []
api_specs:
- filename: consolidated-edison-green-button-connect-openapi.yml
  format: yaml
  label: Green Button Connect My Data
  slug: green-button-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-green-button-connect-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Consolidated Edison Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Consolidated Edison secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Consolidated Edison
provider_slug: consolidated-edison
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://www.coned.com/en/oauth/authorize
    authorizationUrlTest: https://uat10.coned.com/en/oauth/authorize
    description: Customer-consented authorization. The third party redirects the retail customer to the utility authorization server with scope, client_id, redirect_uri, state and response_type; on consent the customer is returned to the third-party redirect URI with an authorization code that is exchanged for an access token and refresh token.
    flow: authorizationCode
    tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token
    tokenUrlTest: https://apit.coned.com/gbc/espi/1_1/oauth/token
  - description: Third-Party Client Access Token (CAT). grant_type=client_credentials with HTTP Basic client_id:client_secret. A CAT retrieves data for all customers currently authorized to the third party, within the granted scope.
    flow: clientCredentials
    tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token
    tokenUrlTest: https://apit.coned.com/gbc/espi/1_1/oauth/token
  - description: grant_type=refresh_token with HTTP Basic client_id:client_secret plus the customer's refresh_token and scope. Used to mint each subsequent one-hour user access token.
    flow: refreshToken
    tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token
  name: GreenButtonOAuth2
  sources:
  - Con Edison GBC Third-Party Technical Onboarding Document v4.4
  standard: NAESB ESPI (REQ.21) OAuth 2.0 profile, RFC 6749 + RFC 6750
  type: oauth2
- description: All /resource/* ESPI operations are called with the OAuth 2.0 bearer access token in the Authorization header (RFC 6750). Unauthorized calls return 401 (observed live against https://api.coned.com/gbc/espi/1_1/resource/ReadServiceStatus).
  name: BearerAccessToken
  scheme: bearer
  sources:
  - openapi/consolidated-edison-green-button-connect-openapi.yml
  type: http
slug: consolidated-edison-authentication
source_filename: consolidated-edison-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://www.coned.com/en/accounts-billing/share-energy-usage-data/become-a-third-party\ndocs: >-\n  https://edge-e-dcxprod-web-bechbkdqagefb9ge.a03.azurefd.net/-/media/files/coned/documents/accountandbilling/share-my-data/onboarding-doc.pdf\nnote: >-\n  Con Edison's Green Button Connect (Share My Data) Swagger definition ships no\n  securityDefinitions block; the OAuth 2.0 model below is taken verbatim from\n  Con Edison's own \"Green Button Connect Third-Party Technical Onboarding\n  Document\" v4.4 (last updated 2026-05-07), which is linked from the public\n  Become a Third Party page.\nsummary:\n  types:\n    - oauth2\n    - http\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\n    - refreshToken\n  bearer: true\nschemes:\n  - name: GreenButtonOAuth2\n    type: oauth2\n    standard: NAESB ESPI (REQ.21) OAuth 2.0 profile, RFC 6749 + RFC 6750\n    sources:\n      - Con Edison GBC\
  \ Third-Party Technical Onboarding Document v4.4\n    flows:\n      - flow: authorizationCode\n        description: >-\n          Customer-consented authorization. The third party redirects the retail\n          customer to the utility authorization server with scope, client_id,\n          redirect_uri, state and response_type; on consent the customer is\n          returned to the third-party redirect URI with an authorization code\n          that is exchanged for an access token and refresh token.\n        authorizationUrl: https://www.coned.com/en/oauth/authorize\n        authorizationUrlTest: https://uat10.coned.com/en/oauth/authorize\n        tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token\n        tokenUrlTest: https://apit.coned.com/gbc/espi/1_1/oauth/token\n      - flow: clientCredentials\n        description: >-\n          Third-Party Client Access Token (CAT). grant_type=client_credentials\n          with HTTP Basic client_id:client_secret. A CAT retrieves data for all\n\
  \          customers currently authorized to the third party, within the granted\n          scope.\n        tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token\n        tokenUrlTest: https://apit.coned.com/gbc/espi/1_1/oauth/token\n      - flow: refreshToken\n        description: >-\n          grant_type=refresh_token with HTTP Basic client_id:client_secret plus\n          the customer's refresh_token and scope. Used to mint each subsequent\n          one-hour user access token.\n        tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token\n  - name: BearerAccessToken\n    type: http\n    scheme: bearer\n    description: >-\n      All /resource/* ESPI operations are called with the OAuth 2.0 bearer\n      access token in the Authorization header (RFC 6750). Unauthorized calls\n      return 401 (observed live against\n      https://api.coned.com/gbc/espi/1_1/resource/ReadServiceStatus).\n    sources:\n      - openapi/consolidated-edison-green-button-connect-openapi.yml\ntoken_lifetimes:\n\
  \  access_token_seconds: 3600\n  access_token_note: >-\n    All access tokens expire in 60 minutes; Con Edison instructs third parties\n    to cache and reuse the token for the same subscription until it expires.\n  refresh_token_expiry: >-\n    A refresh token expires after one year if it is never used to acquire a new\n    access token; recovery requires the customer to revoke and re-authorize.\n  refresh_token_storage: >-\n    Refresh tokens are issued once at authorization time and are not re-issued —\n    a lost refresh token requires customer revocation and re-authorization.\ncredentials:\n  issuance: >-\n    client_id, client_secret and a Registration Access Token are emailed to the\n    third party by Con Edison's GBC technical onboarding team after the\n    registration form and Data Security Agreement are completed. client_id and\n    client_secret can also be retrieved from the ApplicationInformation resource\n    using the Registration Access Token.\n  contact: dlsharemydatatech@coned.com\n\
  \  transport: >-\n    All third-party callback and redirect URLs must be reachable from the Con\n    Edison network and must support TLS 1.2 or higher.\ndata_custodians:\n  - name: Consolidated Edison Company of New York (CECONY)\n    authorization_base: https://www.coned.com/en/\n    api_base: https://api.coned.com/gbc/espi/1_1\n    test_api_base: https://apit.coned.com/gbc/espi/1_1\n  - name: Orange & Rockland Utilities (ORU)\n    authorization_base: https://www.oru.com/en/\n    note: >-\n      Same registration process and API contract; authorization must be routed\n      to the utility that serves the account being authorized.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/authentication/consolidated-edison-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- AMI
- Demand Response
- ESPI
- Energy
- Fortune 500
- Green Button
- Interval Data
- NAESB
- Natural Gas
- New York
- OAuth2
- Steam
- Utility
---
