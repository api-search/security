---
api_key_in:
- body
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kartra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kartra secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kartra
provider_slug: kartra
scheme_count: 3
schemes:
- description: The developer's App identifier, issued when a custom App is created under Settings > Integrations > My Apps and hard-coded into the integration. Kartra rejects any call without a valid App ID.
  errors:
  - 238 App Id cannot be empty
  - 239 App Id is not valid. The app does not exists or is inactive
  - 240 App Account inactive
  held_by: app-developer
  in: body
  name: app_id
  parameter: app_id
  type: apiKey
- description: The end user's Kartra API key, obtained by that user from Settings > Integrations > My API in their own account.
  errors:
  - 202 API key cannot be empty
  - 203 API key not valid
  - 204 API Account inactive
  held_by: app-user
  in: body
  name: api_key
  parameter: api_key
  type: apiKey
- description: The end user's Kartra API password, issued alongside the API key.
  errors:
  - 233 API password not valid. Please get an API password first
  held_by: app-user
  in: body
  name: api_password
  parameter: api_password
  type: apiKey
slug: kartra-authentication
source_filename: kartra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://support.kartra.com/en/articles/15369013-connecting-to-the-api\ndocs:\n- https://support.kartra.com/en/articles/15369013-connecting-to-the-api\n- https://support.kartra.com/en/articles/15369011-activating-your-app\n- https://support.kartra.com/en/articles/15369014-success-and-error-confirmation-messages\nsummary:\n  types: [apiKey]\n  api_key_in: [body]\n  oauth2_flows: []\n  note: >-\n    Kartra's developer API uses no standard HTTP auth scheme. There is no\n    Authorization header, no bearer token and no OAuth2. Three credentials are\n    posted as ordinary form fields in the request body of every call. This is a\n    three-credential model rather than a single key, and it separates the App\n    developer's identity from the App user's account.\ntransport:\n  scheme: https\n  required: true\n  note: >-\n    \"you must connect using https (not http) as our API requires SSL encryption\n    for a request to be accepted.\"\
  \ An http call is rejected with error type 201\n    \"Connection not secure\".\nschemes:\n- name: app_id\n  type: apiKey\n  in: body\n  parameter: app_id\n  held_by: app-developer\n  description: >-\n    The developer's App identifier, issued when a custom App is created under\n    Settings > Integrations > My Apps and hard-coded into the integration.\n    Kartra rejects any call without a valid App ID.\n  errors: ['238 App Id cannot be empty', '239 App Id is not valid. The app does not exists or is inactive', '240 App Account inactive']\n- name: api_key\n  type: apiKey\n  in: body\n  parameter: api_key\n  held_by: app-user\n  description: >-\n    The end user's Kartra API key, obtained by that user from Settings >\n    Integrations > My API in their own account.\n  errors: ['202 API key cannot be empty', '203 API key not valid', '204 API Account inactive']\n- name: api_password\n  type: apiKey\n  in: body\n  parameter: api_password\n  held_by: app-user\n  description: The end user's Kartra\
  \ API password, issued alongside the API key.\n  errors: ['233 API password not valid. Please get an API password first']\nidentity_model:\n  roles:\n  - role: app-developer\n    holds: app_id\n    note: Creator of the third-party integration. The App must be submitted for manual review before it leaves Test Mode.\n  - role: app-user\n    holds: [api_key, api_password]\n    note: >-\n      The Kartra account the actions execute against. \"The actions commanded by\n      the API call will be executed in the App user's Kartra account, not in the\n      App developer's Kartra account.\"\nauthorization:\n  model: per-app-command-permissions\n  note: >-\n    Kartra gates which commands an App may execute. Attempting a command the App\n    is not approved for returns error type 262 \"App does not have permission to\n    execute this CMD\". There is no OAuth scope surface, no consent screen and no\n    published permission catalogue — approval is granted by Kartra admins during\n    App review,\
  \ so the permission set is not machine-discoverable.\n  ip_allowlist:\n    supported: true\n    evidence: 'Error type 242: \"This API call was sent from an unauthorized IP\"'\n    note: Kartra enforces an IP allowlist per App; the configuration surface is inside the account UI and is not documented publicly.\noauth2: null\noauth2_note: >-\n  login.kartra.com runs Auth0 for the Kartra web application's own end-user\n  sign-in (an OIDC authorization_code + PKCE flow observed on the app.kartra.com\n  307). That is the product's human login, NOT an API authorization surface —\n  it issues no developer-usable token and no scopes. Do not read it as OAuth2\n  support for the API.\ngaps:\n- No Authorization header; credentials travel in the POST body of every request.\n- No token issuance, expiry, refresh or revocation is documented.\n- No key-rotation guidance published.\n- No machine-readable securityScheme (Kartra publishes no OpenAPI).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kartra/refs/heads/main/authentication/kartra-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Marketing Automation
- Email Marketing
- CRM
- Contacts
- E-Commerce
- Payments
- Subscription
- Membership
- Landing Pages
- Webhook
- Software-as-a-Service
---
