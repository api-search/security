---
api_key_in:
- header
api_specs:
- filename: treasure-data-bulk-loads-api-openapi.yml
  format: yaml
  label: Treasure Data Bulk Loads API
  slug: treasure-data-bulk-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-bulk-loads-api-openapi.yml
- filename: treasure-data-system-api-openapi.yml
  format: yaml
  label: Treasure Data System API
  slug: treasure-data-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-system-api-openapi.yml
- filename: treasure-data-postback-api-openapi.yml
  format: yaml
  label: Treasure Data Postback API
  slug: treasure-data-postback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-postback-api-openapi.yml
- filename: treasure-data-bulk-import-api-openapi.yml
  format: yaml
  label: Treasure Data Bulk Import API
  slug: treasure-data-bulk-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-bulk-import-api-openapi.yml
- filename: treasure-data-bulk-loads-api-openapi.yml
  format: yaml
  label: Treasure Data Bulk Loads API
  slug: treasure-data-bulk-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-bulk-loads-api-openapi.yml
- filename: treasure-data-connectors-api-openapi.yml
  format: yaml
  label: Treasure Data Connectors API
  slug: treasure-data-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-connectors-api-openapi.yml
- filename: treasure-data-databases-api-openapi.yml
  format: yaml
  label: Treasure Data Databases API
  slug: treasure-data-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-databases-api-openapi.yml
- filename: treasure-data-jobs-api-openapi.yml
  format: yaml
  label: Treasure Data Jobs API
  slug: treasure-data-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-jobs-api-openapi.yml
- filename: treasure-data-sso-api-openapi.yml
  format: yaml
  label: Treasure Data SSO API
  slug: treasure-data-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-sso-api-openapi.yml
- filename: treasure-data-system-api-openapi.yml
  format: yaml
  label: Treasure Data System API
  slug: treasure-data-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-system-api-openapi.yml
- filename: treasure-data-tables-api-openapi.yml
  format: yaml
  label: Treasure Data Tables API
  slug: treasure-data-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-tables-api-openapi.yml
- filename: treasure-data-users-api-openapi.yml
  format: yaml
  label: Treasure Data Users API
  slug: treasure-data-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-users-api-openapi.yml
- filename: treasure-data-td-api-v3-openapi.yml
  format: yaml
  label: Treasure Data API v3
  slug: treasure-data-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-td-api-v3-openapi.yml
- filename: treasure-data-cdp-api-openapi.yml
  format: yaml
  label: Treasure Data CDP API
  slug: treasure-data-cdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-cdp-api-openapi.yml
- filename: treasure-data-llm-api-openapi.yml
  format: yaml
  label: Treasure Data LLM API
  slug: treasure-data-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-llm-api-openapi.yml
- filename: treasure-data-workflow-api-openapi.yml
  format: yaml
  label: Treasure Workflow API
  slug: treasure-data-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-workflow-api-openapi.yml
- filename: treasure-data-dwh-integration-api-openapi.yml
  format: yaml
  label: Treasure Data Data Warehouse Integration API
  slug: treasure-data-dwh-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-dwh-integration-api-openapi.yml
- filename: treasure-data-personalization-api-openapi.yml
  format: yaml
  label: Treasure Data Personalization Service
  slug: treasure-data-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-personalization-api-openapi.yml
- filename: treasure-data-postback-api-openapi.yml
  format: yaml
  label: Treasure Data Postback API
  slug: treasure-data-postback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-postback-api-openapi.yml
- filename: treasure-data-postback-api-v2-openapi.yml
  format: yaml
  label: Treasure Data Postback API v2
  slug: treasure-data-postback-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/openapi/treasure-data-postback-api-v2-openapi.yml
auth_types:
- apiKey
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Treasure Data Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- refresh_token
overview: Treasure Data secures its APIs with apiKey, http, and openIdConnect across 8 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code and refresh_token flow(s).
provider_name: Treasure Data
provider_slug: treasure-data
scheme_count: 8
schemes:
- description: Treasure Data API key. The header value is the literal `TD1` followed by a space and the key, which is an account-number prefix, a slash, and a 40-character hexadecimal string.
  name: ApiKeyAuth
  scheme: TD1
  sources:
  - openapi/treasure-data-td-api-v3-openapi.yml
  - openapi/treasure-data-llm-api-openapi.yml
  - openapi/treasure-data-workflow-api-openapi.yml
  type: http
- description: Same TD1 API key, modelled as an apiKey header scheme by the CDP API spec.
  in: header
  name: TdApikeyAuth
  parameter: Authorization
  sources:
  - openapi/treasure-data-cdp-api-openapi.yml
  type: apiKey
- description: Same TD1 API key, modelled as an apiKey header scheme by the DWH Integration API spec.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/treasure-data-dwh-integration-api-openapi.yml
  type: apiKey
- bearerFormat: TD1
  description: 'The API token is accepted as a `TD1` token. The TD API token

    is an account number prefix, slash, and 40-character

    hexadecimal string.'
  name: td1
  scheme: bearer
  sources:
  - openapi/treasure-data-personalization-api-openapi.yml
  type: http
- description: Web personalization routing token — account number, index number and a 32-character hexadecimal string joined with slashes. Routes the request to the correct real-time engine.
  in: header
  name: wp13n
  parameter: WP13n-Token
  sources:
  - openapi/treasure-data-personalization-api-openapi.yml
  type: apiKey
- description: Write-only ingestion key for the Postback API v2 event endpoint.
  in: header
  name: XTDWriteKey
  parameter: X-TD-Write-Key
  sources:
  - openapi/treasure-data-postback-api-v2-openapi.yml
  type: apiKey
- description: Full TD1 API key accepted as an alternative to the write key on Postback API v2.
  in: header
  name: TD1Authorization
  parameter: Authorization
  sources:
  - openapi/treasure-data-postback-api-v2-openapi.yml
  type: apiKey
- description: TD1 API key as modelled by the API-Evangelist-derived TD API split specs harvested before the provider's own OpenAPI descriptions were located.
  in: header
  name: TDAuth
  parameter: Authorization
  sources:
  - openapi/treasure-data-bulk-import-api-openapi.yml
  - openapi/treasure-data-bulk-loads-api-openapi.yml
  - openapi/treasure-data-connectors-api-openapi.yml
  - openapi/treasure-data-databases-api-openapi.yml
  - openapi/treasure-data-jobs-api-openapi.yml
  - openapi/treasure-data-sso-api-openapi.yml
  - openapi/treasure-data-system-api-openapi.yml
  - openapi/treasure-data-tables-api-openapi.yml
  - openapi/treasure-data-users-api-openapi.yml
  type: apiKey
slug: treasure-data-authentication
source_filename: treasure-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/treasure-data-td-api-v3-openapi.yml, openapi/treasure-data-cdp-api-openapi.yml,\n  openapi/treasure-data-llm-api-openapi.yml, openapi/treasure-data-workflow-api-openapi.yml,\n  openapi/treasure-data-dwh-integration-api-openapi.yml, openapi/treasure-data-personalization-api-openapi.yml,\n  openapi/treasure-data-postback-api-v2-openapi.yml, openapi/treasure-data-postback-api-openapi.yml,\n  well-known/treasure-data-openid-configuration.json\ndocs: https://docs.treasure.ai/tools/cli-and-sdks/configuring-authentication-for-td-using-the-td-toolbelt\nsummary:\n  types:\n  - apiKey\n  - http\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorization_code\n  - refresh_token\n  primary_scheme: >-\n    Static TD API key sent as `Authorization: TD1 <account>/<40-hex>`. Every REST API in the estate uses\n    this one credential; the only variations are how the spec models it (apiKey-in-header vs http scheme\n\
  \    TD1) and the two write-key variants on the ingestion endpoints.\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: TD1\n  description: >-\n    Treasure Data API key. The header value is the literal `TD1` followed by a space and the key, which is\n    an account-number prefix, a slash, and a 40-character hexadecimal string.\n  sources:\n  - openapi/treasure-data-td-api-v3-openapi.yml\n  - openapi/treasure-data-llm-api-openapi.yml\n  - openapi/treasure-data-workflow-api-openapi.yml\n- name: TdApikeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Same TD1 API key, modelled as an apiKey header scheme by the CDP API spec.\n  sources:\n  - openapi/treasure-data-cdp-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Same TD1 API key, modelled as an apiKey header scheme by the DWH Integration API spec.\n  sources:\n  - openapi/treasure-data-dwh-integration-api-openapi.yml\n- name: td1\n  type: http\n\
  \  scheme: bearer\n  bearerFormat: TD1\n  description: |-\n    The API token is accepted as a `TD1` token. The TD API token\n    is an account number prefix, slash, and 40-character\n    hexadecimal string.\n  sources:\n  - openapi/treasure-data-personalization-api-openapi.yml\n- name: wp13n\n  type: apiKey\n  in: header\n  parameter: WP13n-Token\n  description: >-\n    Web personalization routing token — account number, index number and a 32-character hexadecimal\n    string joined with slashes. Routes the request to the correct real-time engine.\n  sources:\n  - openapi/treasure-data-personalization-api-openapi.yml\n- name: XTDWriteKey\n  type: apiKey\n  in: header\n  parameter: X-TD-Write-Key\n  description: Write-only ingestion key for the Postback API v2 event endpoint.\n  sources:\n  - openapi/treasure-data-postback-api-v2-openapi.yml\n- name: TD1Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Full TD1 API key accepted as an alternative to\
  \ the write key on Postback API v2.\n  sources:\n  - openapi/treasure-data-postback-api-v2-openapi.yml\n- name: TDAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    TD1 API key as modelled by the API-Evangelist-derived TD API split specs harvested before the\n    provider's own OpenAPI descriptions were located.\n  sources:\n  - openapi/treasure-data-bulk-import-api-openapi.yml\n  - openapi/treasure-data-bulk-loads-api-openapi.yml\n  - openapi/treasure-data-connectors-api-openapi.yml\n  - openapi/treasure-data-databases-api-openapi.yml\n  - openapi/treasure-data-jobs-api-openapi.yml\n  - openapi/treasure-data-sso-api-openapi.yml\n  - openapi/treasure-data-system-api-openapi.yml\n  - openapi/treasure-data-tables-api-openapi.yml\n  - openapi/treasure-data-users-api-openapi.yml\nopenid_connect:\n  discovery: https://api.treasuredata.com/.well-known/openid-configuration\n  file: well-known/treasure-data-openid-configuration.json\n  issuer: https://console.us01.treasuredata.com\n\
  \  authorization_endpoint: https://console.us01.treasuredata.com/oauth/authorize\n  token_endpoint: https://console.us01.treasuredata.com/oauth/token\n  revocation_endpoint: https://console.us01.treasuredata.com/oauth/revoke\n  introspection_endpoint: https://console.us01.treasuredata.com/oauth/introspect\n  userinfo_endpoint: https://console.us01.treasuredata.com/oauth/userinfo\n  jwks_uri: https://console.us01.treasuredata.com/oauth/discovery/keys\n  grant_types: [authorization_code, refresh_token]\n  response_types: [code]\n  pkce: [plain, S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  claims: [iss, sub, aud, exp, iat, email, email_verified, td_account_id, administrator]\n  note: >-\n    Treasure Data runs an OAuth 2.0 / OpenID Connect authorization server on the console host and\n    advertises it from api.treasuredata.com. None of the eight published OpenAPI descriptions declares an\n    oauth2 securityScheme, so\
  \ OAuth is not (yet) the documented path for calling the REST APIs — it backs\n    console sign-in and third-party app authorization. API calls use the static TD1 key.\nsso:\n  supported: true\n  docs: https://docs.treasure.ai/apis/td-api/identity-federation\n  note: >-\n    SAML identity federation with per-user SSO enforcement is managed through /account/sso_setting and\n    the /user/*_sso endpoints. Multiple IdPs have been supported since the April 2023 release.\nnotes:\n  - >-\n    One credential, many spec shapes. The same TD1 key authenticates the TD API, CDP API, LLM API,\n    Workflow API and DWH Integration API; each spec models it differently, which is a real interoperability\n    friction for generated clients.\n  - >-\n    postback-api (v1) declares no securityScheme at all — the write key travels in the path/payload. v2\n    fixed this with the X-TD-Write-Key header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/authentication/treasure-data-authentication.yml
summary_line: apiKey/http/openIdConnect · 8 schemes
tags:
- Customer Data Platform
- CDP
- Big Data
- Data Warehouse
- Hive
- Presto
- Enterprise
- Artificial Intelligence
- Marketing
- Analytics
---
