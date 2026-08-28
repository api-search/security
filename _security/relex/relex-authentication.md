---
api_key_in: []
api_specs:
- filename: relex-data-api-openapi.json
  format: json
  label: RELEX Data API
  slug: relex-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/openapi/relex-data-api-openapi.json
- filename: relex-monitoring-api-openapi.json
  format: json
  label: RELEX Monitoring API
  slug: relex-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/openapi/relex-monitoring-api-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Relex Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: RELEX Solutions secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: RELEX Solutions
provider_slug: relex
scheme_count: 2
schemes:
- api: RELEX Data API
  applied: globally, via the root `security` requirement — every one of the 91 operations is protected
  description: The RELEX Data API uses OAuth 2 with the client credentials flow.
  flows:
  - flow: clientCredentials
    scopes:
    - openid_api
    tokenUrl: https://identity.prod-eu.prod.cc.relexsolutions.com/login/restapi_prod/connect/token
    tokenUrl_uat: https://identity.prod-eu.prod.cc.relexsolutions.com/login/restapi_uat/connect/token
    tokenUrl_us: https://identity.prod-us.prod.cc.relexsolutions.com/login/restapi_prod/connect/token
  name: OAuth2
  sources:
  - openapi/relex-data-api-openapi.json
  type: oauth2
- api: RELEX Monitoring API
  applied: declared but NOT applied — the spec has no root `security` requirement and no per-operation `security` block, so the contract does not mark any operation as protected even though the docs and the first-party demo client both send a bearer token
  description: OAuth2 client credentials grant; the token endpoint URL depends on the region.
  flows:
  - flow: clientCredentials
    scopes: []
    tokenUrl: https://identity.prod-eu.prod.cc.relexsolutions.com/monitoring_api_prod/connect/token
    tokenUrl_us: https://identity.prod-us.prod.cc.relexsolutions.com/monitoring_api_prod/connect/token
  name: oauth2
  sources:
  - openapi/relex-monitoring-api-openapi.json
  type: oauth2
slug: relex-authentication
source_filename: relex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.relexsolutions.com/api/retail-restapi-example-customer.html\ndocs: https://www.relexsolutions.com/api/retail-restapi-example-customer.html\nderived_from:\n- openapi/relex-data-api-openapi.json\n- openapi/relex-monitoring-api-openapi.json\n- well-known/relex-identity-eu-openid-configuration.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_keys: false\n  basic_auth: false\n  mutual_tls: false\n  self_service: false\n  anonymous_surface:\n  - url: https://us.monitor.relexsolutions.com/\n    what: Monitoring API service-root liveness document\n    note: The only unauthenticated endpoint found on any RELEX host.\nmodel: >-\n  One model across both APIs — OAuth 2.0 Client Credentials against RELEX Identity, an OpenID\n  Connect provider, returning a JWT bearer token. There is no API-key path, no basic auth and no\n  mTLS. Credentials are provisioned by RELEX; there is no signup, console\
  \ or developer registration\n  that issues them.\nschemes:\n- name: OAuth2\n  api: RELEX Data API\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.prod-eu.prod.cc.relexsolutions.com/login/restapi_prod/connect/token\n    tokenUrl_us: https://identity.prod-us.prod.cc.relexsolutions.com/login/restapi_prod/connect/token\n    tokenUrl_uat: https://identity.prod-eu.prod.cc.relexsolutions.com/login/restapi_uat/connect/token\n    scopes:\n    - openid_api\n  applied: globally, via the root `security` requirement — every one of the 91 operations is\n    protected\n  description: The RELEX Data API uses OAuth 2 with the client credentials flow.\n  sources:\n  - openapi/relex-data-api-openapi.json\n- name: oauth2\n  api: RELEX Monitoring API\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.prod-eu.prod.cc.relexsolutions.com/monitoring_api_prod/connect/token\n    tokenUrl_us: https://identity.prod-us.prod.cc.relexsolutions.com/monitoring_api_prod/connect/token\n\
  \    scopes: []\n  applied: 'declared but NOT applied — the spec has no root `security` requirement and no\n    per-operation `security` block, so the contract does not mark any operation as protected even\n    though the docs and the first-party demo client both send a bearer token'\n  description: OAuth2 client credentials grant; the token endpoint URL depends on the region.\n  sources:\n  - openapi/relex-monitoring-api-openapi.json\ntoken_request:\n  method: POST\n  content_type: application/x-www-form-urlencoded\n  body_params:\n  - client_id\n  - client_secret\n  - grant_type=client_credentials\n  client_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  response_fields:\n  - access_token\n  - expires_in\n  - token_type\n  - scope\n  token_type: Bearer\ntoken_use:\n  header: Authorization\n  format: 'Bearer <jwt>'\n  jwt: true\n  jwt_rfc: RFC 7519\n  jwks_uri: https://identity.prod-eu.prod.cc.relexsolutions.com/login/restapi_prod/.well-known/openid-configuration/jwks\n\
  expiry:\n  refresh_tokens: false\n  refresh_note: >-\n    RELEX cites RFC 6749 §4.4.3 directly — the Client Credentials grant is not compatible with\n    refresh tokens. On expiry the API returns 401.\n  client_strategies:\n  - React to 401 by re-running the Client Credentials grant.\n  - Track expires_in and pre-emptively re-issue before it elapses.\ncredential_issuance:\n  self_service: false\n  issued_by: RELEX, during the implementation project\n  required_inputs:\n  - Client ID\n  - Client Secret\n  - RELEX Identity token endpoint URL\n  quote: >-\n    \"To authenticate with RELEX Identity, the client needs a Client ID, a Client Secret and a RELEX\n    Identity token endpoint URL. These are provided by RELEX during the implementation process.\"\n  rotation_policy: not published\ntransport_and_network:\n  https_required: true\n  http_behaviour: plain HTTP requests fail with 400 Bad Request\n  ip_allowlist:\n    supported: true\n    recommended_by_provider: true\n    quote: 'The recommendation\
  \ is to always have an IP allowlist in place.'\n    blocklist_supported: false\n  typical_403_cause: caller's egress IP is not on the allowlist for that environment\nidentity_provider:\n  name: RELEX Identity\n  family: IdentityServer / Duende (OpenID Connect)\n  discovery_documents:\n  - well-known/relex-identity-eu-openid-configuration.json\n  - well-known/relex-identity-eu-restapi-prod-openid-configuration.json\n  - well-known/relex-identity-eu-monitoring-api-prod-openid-configuration.json\n  - well-known/relex-identity-us-openid-configuration.json\n  - well-known/relex-identity-us-restapi-prod-openid-configuration.json\n  - well-known/relex-identity-us-monitoring-api-prod-openid-configuration.json\n  regions:\n  - eu\n  - us\n  authorities_per_region: 3\n  see: scopes/relex-scopes.yml\ndeveloper_portal_auth:\n  url: https://docs.relexsolutions.com/\n  gate: Auth0 via Azure Static Web Apps\n  observed: GET / 302s to /.auth/login/auth0?post_login_redirect_uri=/.auth/complete\n  note:\
  \ >-\n    The full RELEX Developer Portal — which RELEX says carries documentation for every integration\n    method, data formats, authentication, monitoring and the SAP Connector specs — requires a\n    registered account. Everything captured in this repo came from the parts RELEX publishes\n    outside that wall.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/authentication/relex-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Supply Chain
- Retail
- Demand Planning
- Inventory Management
- Forecasting
- Pricing
- Enterprise Software
- Data Integration
- Company
---
