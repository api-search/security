---
api_key_in: []
api_specs:
- filename: mapp-engage-openapi.yml
  format: yaml
  label: Mapp Engage API
  slug: engage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-engage-openapi.yml
- filename: mapp-intelligence-analytics-openapi.yml
  format: yaml
  label: Mapp Intelligence Analytics API
  slug: intelligence-analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-intelligence-analytics-openapi.yml
- filename: mapp-product-catalog-openapi.yml
  format: yaml
  label: Mapp Product Catalog Public API
  slug: product-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-product-catalog-openapi.yml
- filename: mapp-fashion-openapi.yml
  format: yaml
  label: Mapp Fashion API
  slug: fashion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-fashion-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mapp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Mapp Marketing Cloud secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Mapp Marketing Cloud
provider_slug: mapp
scheme_count: 3
schemes:
- description: HTTP Basic authentication with a Mapp Engage system user of type API (or Hybrid).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mapp-engage-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.mapp.com/oauth2/token
  name: oauth_security_scheme
  sources:
  - openapi/mapp-intelligence-analytics-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: Keycloak
  scheme: bearer
  sources:
  - openapi/mapp-product-catalog-openapi.yml
  type: http
slug: mapp-authentication
source_filename: mapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/mapp-engage-openapi.yml, openapi/mapp-intelligence-analytics-openapi.yml, openapi/mapp-product-catalog-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  token_endpoints:\n  - https://auth.mapp.com/oauth2/token\n  mfa_for_api_users: false\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with a Mapp Engage system user of type API (or Hybrid).\n  sources:\n  - openapi/mapp-engage-openapi.yml\n- name: oauth_security_scheme\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.mapp.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/mapp-intelligence-analytics-openapi.yml\n- name: Keycloak\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/mapp-product-catalog-openapi.yml\ndocs:\n- https://docs.mapp.com/apidocs/getting-started-with-engage-api\n\
  - https://docs.mapp.com/apidocs/how-to-grant-access-to-the-intelligence-analytics-api\n- https://docs.mapp.com/apidocs/product-catalog-api-authentification\n- https://docs.mapp.com/docs/mapp-cloud-centralized-api-client-management\n- https://docs.mapp.com/docs/api-client-ids\nnote: 'Four surfaces, four different auth models, one shared credential store. Since 2026-05-28 a single Mapp Cloud\n  API Client ID / Secret (Settings > Mapp Cloud > API Client IDs) works across Connect, Intelligence, Engage and\n  Mapp Fashion, but each service must still be separately enabled on the account by a Customer Success Manager.\n  Mapp Engage is the outlier: it does not use the Client ID at all — it uses HTTP Basic with a system user email\n  and password, sent in clear text (base64) on every request, with no token, no session and no rotation mechanism\n  beyond changing the password. MFA is available for the Mapp Cloud UI but does not apply to API users. Note the\n  breaking detail on the Analytics token\
  \ endpoint: earlier versions required a scope parameter and the current endpoint\n  rejects it.'\nper_api:\n- api: mapp:engage\n  type: http\n  scheme: basic\n  credential: system user (type API or Hybrid) email + password\n  token: null\n  rotation: password change only\n  docs: https://docs.mapp.com/apidocs/getting-started-with-engage-api\n- api: mapp:intelligence-analytics\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://auth.mapp.com/oauth2/token\n  client_auth: HTTP Basic client-id:client-secret\n  token_ttl_default_minutes: 60\n  send_scope_parameter: false\n  docs: https://docs.mapp.com/apidocs/how-to-grant-access-to-the-intelligence-analytics-api\n- api: mapp:product-catalog\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  issuer: Keycloak\n  docs: https://docs.mapp.com/apidocs/product-catalog-api-authentification\n- api: mapp:fashion\n  type: oauth2\n  flow: authorizationCode\n  pkce: required, S256 only\n  redirect_uri: urn:ietf:wg:oauth:2.0:oob:auto\n\
  \  refresh_token: true\n  note: Also references api_key and user_token security schemes that Mapp does not define in the published fragments.\n  docs: https://docs.mapp.com/apidocs/mapp-fashion-api-documentation\n- api: mapp.com MCP endpoint\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  authorization_server: https://mapp.com\n  token_url: https://mapp.com/oauth/token\n  scopes:\n  - mcp\n  dynamic_registration: client_id_metadata_document_supported\n  docs: well-known/mapp-oauth-authorization-server.json\nip_restriction:\n  supported: true\n  docs: https://docs.mapp.com/docs/ip-restriction\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/authentication/mapp-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Marketing
- Marketing Automation
- Email
- Analytics
- Customer Data
- Personalization
- Push Notifications
- SMS
- E-Commerce
- Digital Analytics
- Recommendations
---
