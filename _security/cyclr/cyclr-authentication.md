---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cyclr-account-connector-custom-categories-api-openapi.yml
  format: yaml
  label: Cyclr Account Connector Custom Categories API
  slug: cyclr-account-connector-custom-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connector-custom-categories-api-openapi.yml
- filename: cyclr-account-connector-properties-api-openapi.yml
  format: yaml
  label: Cyclr Account Connector Properties API
  slug: cyclr-account-connector-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connector-properties-api-openapi.yml
- filename: cyclr-account-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Account Connectors API
  slug: cyclr-account-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connectors-api-openapi.yml
- filename: cyclr-account-custom-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Account Custom Connectors API
  slug: cyclr-account-custom-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-custom-connectors-api-openapi.yml
- filename: cyclr-accounts-api-openapi.yml
  format: yaml
  label: Cyclr Accounts API
  slug: cyclr-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-accounts-api-openapi.yml
- filename: cyclr-authentication-api-openapi.yml
  format: yaml
  label: Cyclr Authentication API
  slug: cyclr-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-authentication-api-openapi.yml
- filename: cyclr-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Connectors API
  slug: cyclr-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-connectors-api-openapi.yml
- filename: cyclr-custom-fields-api-openapi.yml
  format: yaml
  label: Cyclr Custom Fields API
  slug: cyclr-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-custom-fields-api-openapi.yml
- filename: cyclr-cycles-api-openapi.yml
  format: yaml
  label: Cyclr Cycles API
  slug: cyclr-cycles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-cycles-api-openapi.yml
- filename: cyclr-edges-api-openapi.yml
  format: yaml
  label: Cyclr Edges API
  slug: cyclr-edges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-edges-api-openapi.yml
- filename: cyclr-mcp-servers-api-openapi.yml
  format: yaml
  label: Cyclr MCP Servers API
  slug: cyclr-mcp-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-mcp-servers-api-openapi.yml
- filename: cyclr-methods-api-openapi.yml
  format: yaml
  label: Cyclr Methods API
  slug: cyclr-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-methods-api-openapi.yml
- filename: cyclr-steps-api-openapi.yml
  format: yaml
  label: Cyclr Steps API
  slug: cyclr-steps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-steps-api-openapi.yml
- filename: cyclr-templates-api-openapi.yml
  format: yaml
  label: Cyclr Templates API
  slug: cyclr-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-templates-api-openapi.yml
- filename: cyclr-transactions-api-openapi.yml
  format: yaml
  label: Cyclr Transactions API
  slug: cyclr-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-transactions-api-openapi.yml
- filename: cyclr-users-api-openapi.yml
  format: yaml
  label: Cyclr Users API
  slug: cyclr-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cyclr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cyclr secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cyclr
provider_slug: cyclr
scheme_count: 3
schemes:
- credential_limit: A Cyclr Console (and a Cyclr Account) can hold up to 20 sets of OAuth Client Credentials.
  description: 'Cyclr''s API uses the OAuth 2.0 Client Credentials flow. The caller exchanges a Client ID and Client Secret at POST {CyclrAPIDomain}/oauth/token (Content-Type application/x-www-form-urlencoded, grant_type=client_credentials) for a bearer Access Token that is sent on subsequent requests as "Authorization: Bearer {access_token}". Access Tokens are valid for 14 days (1,209,600 seconds) by default; multiple active tokens may exist for a single set of Client Credentials and may be revoked individually from the OAuth Client Credentials page in the Cyclr Console.'
  flow: clientCredentials
  name: bearer
  sources:
  - https://community.cyclr.com/user-documentation/api/authentication
  - https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials
  token_endpoint_note: '{CyclrAPIDomain} is region-specific: api.cyclr.com (UK/global), api.us2.cyclr.com (US2), api.cyclr.uk (UK), api.eu.cyclr.com (EU), or a private instance domain.'
  token_lifetime_seconds: 1209600
  token_url: https://{CyclrAPIDomain}/oauth/token
  type: oauth2
- description: For Cyclr API endpoints that operate on a specific Cyclr Account, callers must include the Account's API ID in the X-Cyclr-Account HTTP header alongside the bearer Access Token. The API ID is shown at the top of an Account's Settings page in the Console.
  header_name: X-Cyclr-Account
  in: header
  name: account_header
  sources:
  - https://community.cyclr.com/user-documentation/api/authentication
  - openapi/cyclr-platform-openapi.json
  type: apiKey
- description: Account-level OAuth Client Credentials with an "MCP" scope can additionally have one or more Sign-in Tokens created for them, enabling separate end users to be identified when calling an MCP Server. The Sign-in Token is included as an additional credential during authentication.
  name: account_sign_in_token
  scheme: bearer
  sources:
  - https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials
  type: http
slug: cyclr-authentication
source_filename: cyclr-authentication.yml
source_heading: Authentication Profile
source_url: https://community.cyclr.com/user-documentation/api/authentication
source_yaml: "generated: '2026-11-25'\nmethod: searched\nsource: https://community.cyclr.com/user-documentation/api/authentication\nsources:\n- https://community.cyclr.com/user-documentation/api/authentication\n- https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\n- https://community.cyclr.com/user-documentation/api/introduction-to-the-cyclr-api\n- openapi/cyclr-platform-openapi.json\nsummary:\n  types:\n  - oauth2\n  styles:\n  - bearer\nschemes:\n- name: bearer\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Cyclr's API uses the OAuth 2.0 Client Credentials flow. The caller exchanges\n    a Client ID and Client Secret at POST {CyclrAPIDomain}/oauth/token\n    (Content-Type application/x-www-form-urlencoded, grant_type=client_credentials)\n    for a bearer Access Token that is sent on subsequent requests as\n    \"Authorization: Bearer {access_token}\". Access Tokens are valid for 14 days\n    (1,209,600 seconds) by default;\
  \ multiple active tokens may exist for a single\n    set of Client Credentials and may be revoked individually from the OAuth\n    Client Credentials page in the Cyclr Console.\n  token_url: https://{CyclrAPIDomain}/oauth/token\n  token_endpoint_note: >-\n    {CyclrAPIDomain} is region-specific: api.cyclr.com (UK/global), api.us2.cyclr.com (US2),\n    api.cyclr.uk (UK), api.eu.cyclr.com (EU), or a private instance domain.\n  credential_limit: A Cyclr Console (and a Cyclr Account) can hold up to 20 sets of OAuth\n    Client Credentials.\n  token_lifetime_seconds: 1209600\n  sources:\n  - https://community.cyclr.com/user-documentation/api/authentication\n  - https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\n- name: account_header\n  type: apiKey\n  in: header\n  header_name: X-Cyclr-Account\n  description: >-\n    For Cyclr API endpoints that operate on a specific Cyclr Account, callers\n    must include the Account's API ID in the X-Cyclr-Account\
  \ HTTP header\n    alongside the bearer Access Token. The API ID is shown at the top of an\n    Account's Settings page in the Console.\n  sources:\n  - https://community.cyclr.com/user-documentation/api/authentication\n  - openapi/cyclr-platform-openapi.json\n- name: account_sign_in_token\n  type: http\n  scheme: bearer\n  description: >-\n    Account-level OAuth Client Credentials with an \"MCP\" scope can additionally\n    have one or more Sign-in Tokens created for them, enabling separate end\n    users to be identified when calling an MCP Server. The Sign-in Token is\n    included as an additional credential during authentication.\n  sources:\n  - https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\nlevels:\n- level: console\n  description: Console-level (Partner Console) OAuth Client Credentials grant access\n    to the full Cyclr API.\n  source: https://community.cyclr.com/user-documentation/api/authentication\n- level: account\n  description:\
  \ Account-level OAuth Client Credentials are scoped to a single Cyclr\n    Account and can be restricted with an OAuth Client Scope (\"Webhook\", \"MCP\",\n    or \"Data On Demand\"). Tokens issued from Account-level credentials are only\n    valid for the chosen scope.\n  source: https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\nscopes:\n- name: account:{API_ID}\n  description: Restricts an Access Token obtained with Console-level Client Credentials\n    to a specific Cyclr Account by appending scope=account:{API_ID} on the token\n    request.\n  source: https://community.cyclr.com/user-documentation/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/cyclr/authentication/cyclr-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Connectors
- Custom Connectors
- Data Synchronization
- Embedded iPaaS
- Embedded SaaS Integration
- Embedded UI
- Integration Platform
- Integration
- Marketplace
- Authentication
- REST API
- Software-as-a-Service
- Templates
- Webhook
- White Label
- Workflows
---
