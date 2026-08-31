---
api_key_in: []
api_specs:
- filename: con-edison-applicationinformation-api-openapi.yml
  format: yaml
  label: Con Edison Application Information API
  slug: con-edison-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-applicationinformation-api-openapi.yml
- filename: con-edison-authorization-api-openapi.yml
  format: yaml
  label: Con Edison Authorization API
  slug: con-edison-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-authorization-api-openapi.yml
- filename: con-edison-batch-api-openapi.yml
  format: yaml
  label: Con Edison Batch API
  slug: con-edison-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-batch-api-openapi.yml
- filename: con-edison-electricpowerusagesummary-api-openapi.yml
  format: yaml
  label: Con Edison Electric Power Usage Summary API
  slug: con-edison-electricpowerusagesummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-electricpowerusagesummary-api-openapi.yml
- filename: con-edison-intervalblock-api-openapi.yml
  format: yaml
  label: Con Edison Interval Block API
  slug: con-edison-intervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-intervalblock-api-openapi.yml
- filename: con-edison-localtimeparameters-api-openapi.yml
  format: yaml
  label: Con Edison Local Time Parameters API
  slug: con-edison-localtimeparameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-localtimeparameters-api-openapi.yml
- filename: con-edison-meterreading-api-openapi.yml
  format: yaml
  label: Con Edison Meter Reading API
  slug: con-edison-meterreading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-meterreading-api-openapi.yml
- filename: con-edison-readingtype-api-openapi.yml
  format: yaml
  label: Con Edison Reading Type API
  slug: con-edison-readingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-readingtype-api-openapi.yml
- filename: con-edison-realtimebatch-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Batch API
  slug: con-edison-realtimebatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimebatch-api-openapi.yml
- filename: con-edison-realtimeintervalblock-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Interval Block API
  slug: con-edison-realtimeintervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimeintervalblock-api-openapi.yml
- filename: con-edison-realtimereadingtype-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Reading Type API
  slug: con-edison-realtimereadingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimereadingtype-api-openapi.yml
- filename: con-edison-retailcustomer-api-openapi.yml
  format: yaml
  label: Con Edison Retail Customer API
  slug: con-edison-retailcustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-retailcustomer-api-openapi.yml
- filename: con-edison-servicestatus-api-openapi.yml
  format: yaml
  label: Con Edison Service Status API
  slug: con-edison-servicestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-servicestatus-api-openapi.yml
- filename: con-edison-usagepoint-api-openapi.yml
  format: yaml
  label: Con Edison Usage Point API
  slug: con-edison-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-usagepoint-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Con Edison Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Con Edison secures its APIs with oauth2 and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Con Edison
provider_slug: con-edison
scheme_count: 5
schemes:
- authorization_code_lifetime_seconds: 60
  authorization_code_single_use: true
  authorization_endpoints:
  - custodian: Con Edison
    environment: production
    note: base_url used to build the redirect to the authorization screen
    url: https://www.coned.com/en/
  - custodian: Orange & Rockland
    environment: production
    url: https://www.oru.com/en/
  - custodian: Con Edison
    environment: test
    url: https://uat10.coned.com/en/
  - custodian: Orange & Rockland
    environment: test
    url: https://uat10.oru.com/en/
  client_authentication: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret)'
  declined_authorization_response: '{{Third-Party-Redirect_URI}}?error=access_denied&error_description=Customer denied authorization.&state=123'
  description: Per-customer consent flow. The customer is redirected to the data custodian's authorization screen (Con Edison or Orange & Rockland), selects account, authorization duration and scope, and is redirected back to the third-party redirect URI with an authorization code plus the state value. The third party exchanges the code at the token endpoint for an access token and refresh token.
  flow: authorizationCode
  grant_parameters: grant_type=authorization_code&code=<authorization code>&redirect_uri=<redirect uri>
  name: oauth2-authorization-code
  request_content_type: application/x-www-form-urlencoded
  source_operation: openapi/con-edison-green-button-connect-my-data-swagger.json#Token
  token_endpoints:
  - environment: production
    url: https://api.coned.com/gbc/espi/1_1/oauth/Token
  - environment: test
    url: https://apit.coned.com/gbc/espi/1_1/oauth/token
  token_response_fields:
  - access_token
  - refresh_token
  - token_type
  - expires_in
  - scope
  - resourceURI
  - authorizationURI
  - customerResourceURI
  type: oauth2
- description: Used to mint a new access token for an existing customer authorization once the one-hour access token expires. Con Edison does NOT store the refresh token — if the third party loses it the customer must revoke and re-authorize.
  flow: refreshToken
  grant_parameters: grant_type=refresh_token&refresh_token={refresh_token}&scope=FB=1_3_4_5_7_10_15_16_51_53_56_57_58_60
  name: oauth2-refresh-token
  refresh_token_expiry: 1 year of non-use
  type: oauth2
- description: Third-Party Client Access Token (CAT). Minted from client_id/client_secret and used to retrieve data across ALL customers actively authorized with the third party (usage, billing, account and authorization resources, bounded by each customer's granted scope). Used for the bulk/batch resources.
  flow: clientCredentials
  grant_parameters: grant_type=client_credentials&scope=FB=34_35
  name: oauth2-client-credentials
  token_endpoints:
  - environment: production
    url: https://api.coned.com/gbc/espi/1_1/oauth/Token
  - environment: test
    url: https://apit.coned.com/gbc/espi/1_1/oauth/token
  type: oauth2
- applies_to: all 36 /resource/* operations in the published Swagger definition
  bearer_format: OAuth 2.0 Bearer Token (RFC 6750)
  description: All /resource/* calls carry the access token as an HTTP Bearer token. An anonymous call to https://api.coned.com/gbc/espi/1_1/resource/ReadServiceStatus returns HTTP 401; the token endpoint returns {"Message":"Unauthorized. Access token is missing or invalid."}.
  name: bearer-token
  scheme: bearer
  type: http
- description: A separate Registration Access Token, emailed to the third party after onboarding, is used to retrieve the ApplicationInformation resource (client_id, client_secret, endpoints, notify URIs).
  name: registration-access-token
  scheme: bearer
  source_operation: openapi/con-edison-green-button-connect-my-data-swagger.json#getThirdPartyApplicationById
  type: http
slug: con-edison-authentication
source_filename: con-edison-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://www.coned.com/-/media/files/coned/documents/accountandbilling/share-my-data/onboarding-doc.pdf\ndocs: https://www.coned.com/en/accounts-billing/share-energy-usage-data/become-a-third-party\nnote: >-\n  The published Swagger 2.0 definition (openapi/con-edison-green-button-connect-my-data-swagger.json)\n  declares NO securityDefinitions, so nothing was derivable from the contract. Everything below is\n  taken verbatim from Con Edison's own \"Con Edison/Orange & Rockland Green Button Connect Third-Party\n  Technical Onboarding Document\" (Document Version 4.4, Last Update Date 5/7/2026) and the \"Share My\n  Data FAQ for Third Party Vendors\", both publicly downloadable. Credentials themselves are NOT\n  self-serve: client_id, client_secret and the Registration Access Token are emailed by the Con Edison\n  onboarding team after a signed Data Security Agreement and supervised certification testing.\nsummary:\n  types: [oauth2,\
  \ http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  http_schemes: [basic, bearer]\n  transport: HTTPS only, TLS 1.2 or higher required on all third-party URLs\n  standards: [RFC 6749, RFC 6750, NAESB REQ.21 ESPI]\nschemes:\n- name: oauth2-authorization-code\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    Per-customer consent flow. The customer is redirected to the data custodian's authorization screen\n    (Con Edison or Orange & Rockland), selects account, authorization duration and scope, and is\n    redirected back to the third-party redirect URI with an authorization code plus the state value.\n    The third party exchanges the code at the token endpoint for an access token and refresh token.\n  authorization_endpoints:\n  - environment: production\n    custodian: Con Edison\n    url: https://www.coned.com/en/\n    note: base_url used to build the redirect to the authorization screen\n  - environment: production\n  \
  \  custodian: Orange & Rockland\n    url: https://www.oru.com/en/\n  - environment: test\n    custodian: Con Edison\n    url: https://uat10.coned.com/en/\n  - environment: test\n    custodian: Orange & Rockland\n    url: https://uat10.oru.com/en/\n  token_endpoints:\n  - environment: production\n    url: https://api.coned.com/gbc/espi/1_1/oauth/Token\n  - environment: test\n    url: https://apit.coned.com/gbc/espi/1_1/oauth/token\n  client_authentication: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret)'\n  request_content_type: application/x-www-form-urlencoded\n  grant_parameters: grant_type=authorization_code&code=<authorization code>&redirect_uri=<redirect uri>\n  authorization_code_lifetime_seconds: 60\n  authorization_code_single_use: true\n  token_response_fields: [access_token, refresh_token, token_type, expires_in, scope, resourceURI, authorizationURI, customerResourceURI]\n  declined_authorization_response: >-\n    {{Third-Party-Redirect_URI}}?error=access_denied&error_description=Customer\
  \ denied\n    authorization.&state=123\n  source_operation: openapi/con-edison-green-button-connect-my-data-swagger.json#Token\n- name: oauth2-refresh-token\n  type: oauth2\n  flow: refreshToken\n  description: >-\n    Used to mint a new access token for an existing customer authorization once the one-hour access\n    token expires. Con Edison does NOT store the refresh token — if the third party loses it the\n    customer must revoke and re-authorize.\n  grant_parameters: grant_type=refresh_token&refresh_token={refresh_token}&scope=FB=1_3_4_5_7_10_15_16_51_53_56_57_58_60\n  refresh_token_expiry: 1 year of non-use\n- name: oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Third-Party Client Access Token (CAT). Minted from client_id/client_secret and used to retrieve\n    data across ALL customers actively authorized with the third party (usage, billing, account and\n    authorization resources, bounded by each customer's granted scope). Used for\
  \ the bulk/batch\n    resources.\n  grant_parameters: grant_type=client_credentials&scope=FB=34_35\n  token_endpoints:\n  - environment: production\n    url: https://api.coned.com/gbc/espi/1_1/oauth/Token\n  - environment: test\n    url: https://apit.coned.com/gbc/espi/1_1/oauth/token\n- name: bearer-token\n  type: http\n  scheme: bearer\n  bearer_format: OAuth 2.0 Bearer Token (RFC 6750)\n  description: >-\n    All /resource/* calls carry the access token as an HTTP Bearer token. An anonymous call to\n    https://api.coned.com/gbc/espi/1_1/resource/ReadServiceStatus returns HTTP 401; the token endpoint\n    returns {\"Message\":\"Unauthorized. Access token is missing or invalid.\"}.\n  applies_to: all 36 /resource/* operations in the published Swagger definition\n- name: registration-access-token\n  type: http\n  scheme: bearer\n  description: >-\n    A separate Registration Access Token, emailed to the third party after onboarding, is used to\n    retrieve the ApplicationInformation\
  \ resource (client_id, client_secret, endpoints, notify URIs).\n  source_operation: openapi/con-edison-green-button-connect-my-data-swagger.json#getThirdPartyApplicationById\ntoken_lifetimes:\n  access_token_seconds: 3600\n  access_token_caching: required — \"Third-party should cache the access token and reuse the access token for subsequent API calls until the access token expires\"\n  refresh_token: expires after 1 year if unused\n  authorization_code_seconds: 60\n  authorization_inactivity_revocation_days: 365\ncredential_issuance:\n  self_serve: false\n  process:\n  - Complete the online Third-Party Company Registration Form (separately for Orange & Rockland)\n  - Complete and sign the Data Security Agreement and accept terms and conditions\n  - Submit the technical onboarding registration form (all supplied URLs must be reachable from the Con Edison network and support TLS 1.2+)\n  - Receive client_id, client_secret and Registration Access Token by email from the onboarding team\n\
  \  - Complete supervised testing in the test environment and submit the API testing checklist\n  - Re-register with production details\n  timeline: 30 to 60 days for technical onboarding; 90 days to complete registration testing\n  contacts: [ShareMyData@coned.com, ShareMyDataTech@coned.com, dlsharemydatatech@coned.com]\nnot_supported:\n  openid_connect: https://www.coned.com/.well-known/openid-configuration and https://api.coned.com/.well-known/openid-configuration both return HTTP 404 (probed 2026-07-27)\n  mutual_tls: not documented\n  api_keys: not used\n  accreditation_scheme: none — bilateral utility agreement, not CDR-style accreditation\nopen_surfaces:\n- api: Con Edison Hosting Capacity Map REST API\n  authentication: none — ArcGIS feature services at https://services.arcgis.com/ciPnsNFi1JLWVjva/arcgis/rest/services answer anonymously (HTTP 200)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/authentication/con-edison-authentication.yml
summary_line: oauth2/http · 5 schemes
tags:
- Energy
- United States
- New York
- Utilities
- Electricity
- Gas
- Steam
- Smart Metering
- Green Button
- Energy Data
- Grid
- Distribution
- Hosting Capacity
- Distributed Energy Resources
- Solar
- EV Charging
- Demand Response
---
