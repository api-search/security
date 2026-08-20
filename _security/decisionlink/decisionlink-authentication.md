---
api_key_in: []
api_specs:
- filename: decisionlink-value-proposition-openapi.yml
  format: yaml
  label: Xfactor.io Value Proposition API
  slug: xfactorio-value-proposition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/openapi/decisionlink-value-proposition-openapi.yml
- filename: decisionlink-value-facts-openapi.yml
  format: yaml
  label: Xfactor.io Value Facts API
  slug: xfactorio-value-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/openapi/decisionlink-value-facts-openapi.yml
- filename: decisionlink-value-chat-openapi.yml
  format: yaml
  label: Xfactor.io Value Chat API
  slug: xfactorio-value-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/openapi/decisionlink-value-chat-openapi.yml
- filename: decisionlink-collaboration-openapi.yml
  format: yaml
  label: Xfactor.io Collaboration Manager API
  slug: xfactorio-collaboration-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/openapi/decisionlink-collaboration-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Decisionlink Authentication
name_suffix: Authentication
oauth_flows: []
overview: DecisionLink secures its APIs with http, oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DecisionLink
provider_slug: decisionlink
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'Access token in the form of a JWT. Declared in every one of the four service specs and applied to 146 of 156 operations. Unauthenticated calls return HTTP 401 or 403 with {"detail":"Not authenticated"} and a WWW-Authenticate: Bearer challenge.'
  method: derived
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/decisionlink-collaboration-openapi.yml
  - openapi/decisionlink-value-chat-openapi.yml
  - openapi/decisionlink-value-facts-openapi.yml
  - openapi/decisionlink-value-proposition-openapi.yml
  type: http
- authorization_endpoint: https://xf-prd.us.auth0.com/authorize
  description: The Xfactor.io web application authenticates through a dedicated Auth0 tenant using @auth0/auth0-spa-js and @auth0/auth0-react, then presents the resulting JWT as the bearer token on api.xfactor.io. The token audience observed in the shipped application bundle is the API host itself (https://api.<env>.xfactor.io/), so the API is registered as an Auth0 API resource server.
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://xf-prd.us.auth0.com/
  jwks_uri: https://xf-prd.us.auth0.com/.well-known/jwks.json
  method: probed
  name: Auth0 OIDC (web application)
  note: These are the standard OIDC scopes the Auth0 tenant advertises, not product scopes. No Xfactor.io permission or scope reference is published, so scopes/ is not emitted.
  openIdConnectUrl: https://xf-prd.us.auth0.com/.well-known/openid-configuration
  scopes_supported:
  - openid
  - profile
  - offline_access
  - email
  source: https://xf-prd.us.auth0.com/.well-known/openid-configuration
  token_endpoint: https://xf-prd.us.auth0.com/oauth/token
  type: openIdConnect
  userinfo_endpoint: https://xf-prd.us.auth0.com/userinfo
- description: '"Authentication and authorization for API based access is performed through the use of API keys. XFactor uses one-way hash functions (SHA256) and only stores the hashed version of those keys." Quoted verbatim from the Data Processing Addendum. Key issuance, header name, rotation and expiry are not published anywhere public; they are available to contracted customers only.'
  header: unknown
  method: searched
  name: API keys (API-based access)
  source: https://www.xfactor.io/data-processing-addendum/
  storage: SHA-256 one-way hash (provider statement)
  type: apiKey
slug: decisionlink-authentication
source_filename: decisionlink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.xfactor.io/data-processing-addendum/\ndocs: https://www.xfactor.io/data-processing-addendum/\nnote: >-\n  DecisionLink now trades as Xfactor.io. There is no developer portal and no published\n  authentication guide. The only prose the company publishes about API authentication is in its\n  Data Processing Addendum; the machine-readable half was derived from the four FastAPI OpenAPI 3.1\n  documents served anonymously at api.xfactor.io and from the Auth0 tenant its own web application\n  bundle names as the issuer.\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  - apiKey\n  primary: Auth0-issued OAuth 2.0 / OIDC bearer JWT for application access; hashed API keys for\n    API-based access issued to contracted customers.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Access token in the form of a JWT. Declared in every one of the four service\
  \ specs and applied\n    to 146 of 156 operations. Unauthenticated calls return HTTP 401 or 403 with\n    {\"detail\":\"Not authenticated\"} and a WWW-Authenticate: Bearer challenge.\n  method: derived\n  sources:\n  - openapi/decisionlink-collaboration-openapi.yml\n  - openapi/decisionlink-value-chat-openapi.yml\n  - openapi/decisionlink-value-facts-openapi.yml\n  - openapi/decisionlink-value-proposition-openapi.yml\n- name: Auth0 OIDC (web application)\n  type: openIdConnect\n  openIdConnectUrl: https://xf-prd.us.auth0.com/.well-known/openid-configuration\n  description: >-\n    The Xfactor.io web application authenticates through a dedicated Auth0 tenant using\n    @auth0/auth0-spa-js and @auth0/auth0-react, then presents the resulting JWT as the bearer token\n    on api.xfactor.io. The token audience observed in the shipped application bundle is the API\n    host itself (https://api.<env>.xfactor.io/), so the API is registered as an Auth0 API resource\n    server.\n  method: probed\n\
  \  source: https://xf-prd.us.auth0.com/.well-known/openid-configuration\n  issuer: https://xf-prd.us.auth0.com/\n  authorization_endpoint: https://xf-prd.us.auth0.com/authorize\n  token_endpoint: https://xf-prd.us.auth0.com/oauth/token\n  userinfo_endpoint: https://xf-prd.us.auth0.com/userinfo\n  jwks_uri: https://xf-prd.us.auth0.com/.well-known/jwks.json\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  scopes_supported:\n  - openid\n  - profile\n  - offline_access\n  - email\n  note: >-\n    These are the standard OIDC scopes the Auth0 tenant advertises, not product scopes. No\n    Xfactor.io permission or scope reference is published, so scopes/ is not emitted.\n- name: API keys (API-based access)\n  type: apiKey\n  description: >-\n    \"Authentication and authorization for API based access\
  \ is performed through the use of API\n    keys. XFactor uses one-way hash functions (SHA256) and only stores the hashed version of those\n    keys.\" Quoted verbatim from the Data Processing Addendum. Key issuance, header name, rotation\n    and expiry are not published anywhere public; they are available to contracted customers only.\n  method: searched\n  source: https://www.xfactor.io/data-processing-addendum/\n  storage: SHA-256 one-way hash (provider statement)\n  header: unknown\nenvironments:\n- name: production\n  api_host: https://api.xfactor.io\n  issuer: https://xf-prd.us.auth0.com/\n- name: demo\n  api_host: https://api.demo.xfactor.io\n  issuer: https://xf-demo.us.auth0.com/\n- name: uat\n  api_host: https://api.uat.xfactor.io\n  issuer: https://xf-uat.us.auth0.com/\n- name: sandbox\n  api_host: https://api.snd.xfactor.io\n  issuer: https://xf-sandbox.us.auth0.com/\n- name: development\n  api_host: https://api.dev.xfactor.io\n  issuer: https://xf-dev.us.auth0.com/\nnote_environments:\
  \ >-\n  Non-production hosts are named in the public application bundle at app.xfactor.io. They are the\n  company's own internal environments, not a published developer sandbox — no test credentials,\n  fixtures, or self-service signup exist, so sandbox/ is not emitted.\nhuman_authentication:\n  web_app: passwordless authentication and SSO/SAML\n  source: https://www.xfactor.io/data-processing-addendum/\n  quote: >-\n    Authentication and authorization for webapp based access is performed through industry\n    best-practices including password less authentication and SSO/SAML.\ntransport:\n  tls_minimum: TLS 1.2\n  source: https://www.xfactor.io/data-processing-addendum/\nevidence:\n- url: https://api.xfactor.io/v2/credentials/available-providers\n  status: 401\n  body: '{\"detail\":\"Not authenticated\"}'\n  headers:\n    www-authenticate: Bearer\n- url: https://api.xfactor.io/v1/value-proposition/me\n  status: 403\n  body: '{\"detail\":\"Not authenticated\"}'\n- url: https://xf-prd.us.auth0.com/.well-known/openid-configuration\n\
  \  status: 200\n- url: https://www.xfactor.io/data-processing-addendum/\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decisionlink/refs/heads/main/authentication/decisionlink-authentication.yml
summary_line: http/oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Cloud Saas
- Revenue Operations
- Customer Value Management
- Artificial Intelligence
- Go-To-Market
- Sales
- Analytics
- Value Selling
- Forecasting
---
