---
anonymous_access: false
api_key_in:
- header
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 75F Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: 75F secures its APIs with oauth2, http, and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: 75F
provider_slug: 75f
scheme_count: 2
schemes:
- description: Product-scoped Azure API Management subscription key. Issued per product subscription in the 75F developer portal, or read from Facilisight under Building Options > API Management. Missing or invalid keys are rejected at the gateway with HTTP 401 and never reach the backend.
  in: header
  key_categories:
  - name: Read API
    purpose: retrieve information from the 75F platform
  - name: Write API
    purpose: modify or write information to the platform
  - name: Special Schedule API
    purpose: schedule-related operations
  name: ApimSubscriptionKey
  parameter_name: Ocp-Apim-Subscription-Key
  required: true
  rotation:
    mechanism: two interchangeable keys per API category, rotated without downtime
    source: https://support.75f.io/hc/en-us/articles/54874674979603-API-Management-Via-Facilisight-Application
    supported: true
  sources:
  - https://support.75f.io/hc/en-us/articles/5460365803027-75F-API-s-Error-Returns
  type: apiKey
- description: POST to the token endpoint with grant_type=client_credentials; client_id is the 75F Facilisight username and client_secret is the Facilisight password. The account must be a standard username/password Facilisight account — accounts federated to O365 or Google cannot be used from the API. Returns a JWT access token, token_type bearer.
  flows:
  - flow: clientCredentials
    scopes:
      schedules:read: Read special schedules (v2 Scheduling API)
      schedules:write: Create, update and delete special schedules (v2 Scheduling API)
    tokenUrl: https://api.75f.io/oauth/token
  name: OAuth2ClientCredentials
  required: true
  sources:
  - https://support.75f.io/hc/en-us/articles/5459701361427-Oauth-API
  token:
    expires_in_seconds: 3600
    format: JWT
    header: 'Authorization: Bearer <token>'
    note: The docs state the token response carries expires_in 3600 while the client application credentials themselves expire within 24 hours and require reactivation.
  type: oauth2
slug: 75f-authentication
source_filename: 75f-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://support.75f.io/hc/en-us/articles/5459701361427-Oauth-API\ndocs: https://support.75f.io/hc/en-us/articles/5459584919059-External-Users-API-Developer-Portal\nnote: >-\n  Derived from 75F's own published API documentation rather than from an OpenAPI file: 75F publishes no\n  public machine-readable spec. Two credentials are required on every call — a product-scoped Azure API\n  Management subscription key AND an OAuth 2.0 bearer token minted from Facilisight account credentials.\nsummary:\n  types: [oauth2, http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  two_factor_credentials: true\nschemes:\n- name: ApimSubscriptionKey\n  type: apiKey\n  in: header\n  parameter_name: Ocp-Apim-Subscription-Key\n  required: true\n  description: >-\n    Product-scoped Azure API Management subscription key. Issued per product subscription in the 75F\n    developer portal, or read from Facilisight under Building\
  \ Options > API Management. Missing or\n    invalid keys are rejected at the gateway with HTTP 401 and never reach the backend.\n  rotation:\n    supported: true\n    mechanism: two interchangeable keys per API category, rotated without downtime\n    source: https://support.75f.io/hc/en-us/articles/54874674979603-API-Management-Via-Facilisight-Application\n  key_categories:\n  - {name: Read API, purpose: retrieve information from the 75F platform}\n  - {name: Write API, purpose: modify or write information to the platform}\n  - {name: Special Schedule API, purpose: schedule-related operations}\n  sources: [https://support.75f.io/hc/en-us/articles/5460365803027-75F-API-s-Error-Returns]\n- name: OAuth2ClientCredentials\n  type: oauth2\n  required: true\n  description: >-\n    POST to the token endpoint with grant_type=client_credentials; client_id is the 75F Facilisight\n    username and client_secret is the Facilisight password. The account must be a standard\n    username/password Facilisight\
  \ account — accounts federated to O365 or Google cannot be used from\n    the API. Returns a JWT access token, token_type bearer.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.75f.io/oauth/token\n    scopes:\n      schedules:read: Read special schedules (v2 Scheduling API)\n      schedules:write: Create, update and delete special schedules (v2 Scheduling API)\n  token:\n    format: JWT\n    expires_in_seconds: 3600\n    header: 'Authorization: Bearer <token>'\n    note: >-\n      The docs state the token response carries expires_in 3600 while the client application\n      credentials themselves expire within 24 hours and require reactivation.\n  sources: [https://support.75f.io/hc/en-us/articles/5459701361427-Oauth-API]\nauthorization_model:\n  description: >-\n    Data access is scoped by Facilisight site membership, not by API scopes. An API consumer must hold a\n    Facilisight \"Secondary Manager\" account on every site they intend to read or write; the site\n \
  \   administrator grants it. Requesting points the user is not entitled to returns HTTP 200 with an\n    empty Haystack grid rather than a 403.\n  role_required: Secondary Manager\n  granted_by: the customer's Facilisight account administrator\n  source: https://support.75f.io/hc/en-us/articles/5509604551443-Accessing-the-API\nonboarding:\n  steps:\n  - Register on the 75F developer portal (Azure API Management)\n  - Request a subscription to a published product; a 75F portal admin approves it\n  - Copy the subscription key from the portal profile page (or Facilisight > API Management > API Keys)\n  - Obtain a Facilisight Secondary Manager account for every site in scope\n  - POST client_credentials to /oauth/token to mint a bearer token\n  portal: https://api-management-75f-dev.developer.azure-api.net/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/75f/refs/heads/main/authentication/75f-authentication.yml
summary_line: oauth2/http/apiKey · 2 schemes
tags:
- Company
- Building Automation
- Smart Buildings
- HVAC
- Internet of Things
- Energy Management
- Project Haystack
- Facilities Management
- Sensors
- Building Management System
---
