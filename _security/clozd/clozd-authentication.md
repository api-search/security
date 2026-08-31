---
api_key_in:
- header
api_specs:
- filename: clozd-programs-api-openapi.yml
  format: yaml
  label: Clozd /programs API
  slug: clozd-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-api-openapi.yml
- filename: clozd-programs-program-id-competitors-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/competitors API
  slug: clozd-programs-program-id-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-competitors-api-openapi.yml
- filename: clozd-programs-program-id-deals-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals API
  slug: clozd-programs-program-id-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-api-openapi.yml
- filename: clozd-programs-program-id-deals-deal-id-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals/:deal ID API
  slug: clozd-programs-program-id-deals-deal-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-deal-id-api-openapi.yml
- filename: clozd-programs-program-id-deals-import-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals/import API
  slug: clozd-programs-program-id-deals-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-import-api-openapi.yml
- filename: clozd-programs-program-id-touchpoints-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/touchpoints API
  slug: clozd-programs-program-id-touchpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-touchpoints-api-openapi.yml
- filename: clozd-programs-program-id-touchpoints-touchpoint-id-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/touchpoints/:touchpoint ID API
  slug: clozd-programs-program-id-touchpoints-touchpoint-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-touchpoints-touchpoint-id-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Clozd Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Clozd secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Clozd
provider_slug: clozd
scheme_count: 3
schemes:
- applies_to:
  - Clozd Data API v1.0
  - Clozd Data API v2.0
  - Clozd Data API v3.0
  in: header
  name: apiKey
  parameter: x-api-token
  provisioning:
    display_once: true
    display_once_note: The access token is shown exactly once at creation; if lost a new token must be created. Clozd documents no token rotation schedule, no expiry, and no revocation API.
    docs: https://help.clozd.com/hc/en-us/articles/9948957669659-API-Imports-Exports
    expiry: not-published
    rotation_policy: not-published
    scope: organization
    self_serve: false
    steps:
    - Ask a Clozd Program Manager or support@clozd.com to enable the API Imports setting for the organization.
    - In the Clozd app, open the user menu (initials, top-right) and choose Settings.
    - Scroll to the API Token section, where the Organization ID and each Program ID are shown.
    - Click Create Access Token, name it, and confirm.
  sources:
  - openapi/clozd-data-api-v1-openapi.yml
  - openapi/clozd-data-api-v2-openapi.yml
  - openapi/clozd-data-api-v3-openapi.yml
  type: apiKey
- applies_to:
  - Clozd MCP Server
  client_id_metadata_document_supported: true
  dynamic_client_registration: https://oauth.clozd.com/register
  flows:
  - authorizationUrl: https://oauth.clozd.com/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    scopes:
    - openid
    - profile
    - email
    - offline_access
    - api
    tokenUrl: https://oauth.clozd.com/token
  - flow: clientCredentials
    tokenUrl: https://oauth.clozd.com/token
  - flow: refreshToken
    tokenUrl: https://oauth.clozd.com/token
  issuer: https://oauth.clozd.com
  name: oauth2
  sources:
  - https://oauth.clozd.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- applies_to:
  - Clozd MCP Server
  - Clozd platform SSO
  id_token_signing_alg:
  - RS256
  name: openIdConnect
  openIdConnectUrl: https://oauth.clozd.com/.well-known/openid-configuration
  response_types:
  - code
  sources:
  - https://oauth.clozd.com/.well-known/openid-configuration
  subject_types:
  - public
  type: openIdConnect
slug: clozd-authentication
source_filename: clozd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: >-\n  openapi/clozd-data-api-v1-openapi.yml, openapi/clozd-data-api-v2-openapi.yml,\n  openapi/clozd-data-api-v3-openapi.yml, https://oauth.clozd.com/.well-known/oauth-authorization-server\ndocs:\n- https://help.clozd.com/hc/en-us/articles/9948957669659-API-Imports-Exports\n- https://help.clozd.com/hc/en-us/articles/49656607624987-Connecting-to-Clozd-via-MCP\n- https://help.clozd.com/hc/en-us/articles/45409542002587-Single-Sign-On-SSO\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  note: >-\n    Two distinct auth models by surface. The REST Data API uses a long-lived organization API token in the\n    x-api-token header. The MCP server uses OAuth 2.0 authorization code + PKCE against oauth.clozd.com,\n    which brokers to the customer's own identity provider — no key material is stored in client config.\n\
  schemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-token\n  applies_to:\n  - Clozd Data API v1.0\n  - Clozd Data API v2.0\n  - Clozd Data API v3.0\n  sources:\n  - openapi/clozd-data-api-v1-openapi.yml\n  - openapi/clozd-data-api-v2-openapi.yml\n  - openapi/clozd-data-api-v3-openapi.yml\n  provisioning:\n    docs: https://help.clozd.com/hc/en-us/articles/9948957669659-API-Imports-Exports\n    self_serve: false\n    steps:\n    - Ask a Clozd Program Manager or support@clozd.com to enable the API Imports setting for the organization.\n    - In the Clozd app, open the user menu (initials, top-right) and choose Settings.\n    - Scroll to the API Token section, where the Organization ID and each Program ID are shown.\n    - Click Create Access Token, name it, and confirm.\n    scope: organization\n    display_once: true\n    display_once_note: >-\n      The access token is shown exactly once at creation; if lost a new token must be created. Clozd\n      documents no\
  \ token rotation schedule, no expiry, and no revocation API.\n    rotation_policy: not-published\n    expiry: not-published\n- name: oauth2\n  type: oauth2\n  applies_to:\n  - Clozd MCP Server\n  issuer: https://oauth.clozd.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.clozd.com/authorize\n    tokenUrl: https://oauth.clozd.com/token\n    pkce_methods:\n    - S256\n    scopes:\n    - openid\n    - profile\n    - email\n    - offline_access\n    - api\n  - flow: clientCredentials\n    tokenUrl: https://oauth.clozd.com/token\n  - flow: refreshToken\n    tokenUrl: https://oauth.clozd.com/token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  dynamic_client_registration: https://oauth.clozd.com/register\n  client_id_metadata_document_supported: true\n  sources:\n  - https://oauth.clozd.com/.well-known/oauth-authorization-server\n- name: openIdConnect\n  type: openIdConnect\n  applies_to:\n  - Clozd MCP Server\n \
  \ - Clozd platform SSO\n  openIdConnectUrl: https://oauth.clozd.com/.well-known/openid-configuration\n  id_token_signing_alg:\n  - RS256\n  subject_types:\n  - public\n  response_types:\n  - code\n  sources:\n  - https://oauth.clozd.com/.well-known/openid-configuration\nresource_protection:\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  metadata_url: https://mcp.clozd.com/.well-known/oauth-protected-resource/mcp\n  advertised_via_www_authenticate: true\n  www_authenticate: >-\n    Bearer realm=\"Clozd MCP\",\n    resource_metadata=\"https://mcp.clozd.com/.well-known/oauth-protected-resource/mcp\"\n  bearer_methods_supported:\n  - header\nplatform_sso:\n  supported: true\n  protocols:\n  - SAML 2.0\n  - OIDC\n  identity_providers_documented:\n  - Okta\n  - Microsoft Entra\n  - OneLogin\n  - Google\n  docs:\n  - https://help.clozd.com/hc/en-us/articles/45409542002587-Single-Sign-On-SSO\n  - https://help.clozd.com/hc/en-us/articles/45094828124827-Configuring-OIDC-for-Authentication-with-Okta\n\
  \  - https://help.clozd.com/hc/en-us/articles/45717687212059-Setting-up-SAML-Based-SSO-with-OneLogin\n  - https://help.clozd.com/hc/en-us/articles/45760689187867-Setting-up-SAML-Based-SSO-with-Entra\ngaps:\n- The REST Data API has no OAuth option — only a long-lived, organization-wide, non-expiring API token.\n- No documented token rotation, expiry or programmatic revocation for the REST API token.\n- No read-only vs read-write token distinction on the REST surface.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://oauth.clozd.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.clozd.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n  - url: https://app.clozd.com/public-api/v3/openapi.json\n    http_status: 401\n    body: '{\"success\":false,\"message\":\"API Token Required.\",\"errorCode\":\"API003\"}'\n  - url: https://help.clozd.com/api/v2/help_center/en-us/articles/9948957669659.json\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/authentication/clozd-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- win-loss-analysis
- customer-feedback
- decision-intelligence
- sales-intelligence
- market-research
- Competitive Intelligence
- voice-of-customer
- revenue-intelligence
- saas
- MCP
- agent-native
---
