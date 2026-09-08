---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: devportal-factiva-products
  format: yaml
  label: Dow Jones Developer Platform
  slug: dow-jones-developer-platform
  spec_type: Postman
  url: https://www.postman.com/dj-cse/workspace/devportal-factiva-products
- filename: dow-jones-developer-platform-newswires-real-time-api-openapi.yml
  format: yaml
  label: Dow Jones Newswires Real-Time API
  slug: newswires-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-newswires-real-time-api-openapi.yml
- filename: dow-jones-developer-platform-newswires-top-stories-api-openapi.yml
  format: yaml
  label: Dow Jones Newswires Top Stories API
  slug: newswires-top-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-newswires-top-stories-api-openapi.yml
- filename: dow-jones-developer-platform-calendar-live-api-openapi.yml
  format: yaml
  label: Dow Jones Calendar Live API
  slug: calendar-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-calendar-live-api-openapi.yml
- filename: dow-jones-developer-platform-factiva-content-api-openapi.yml
  format: yaml
  label: Factiva Content API
  slug: factiva-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-factiva-content-api-openapi.yml
- filename: dow-jones-developer-platform-factiva-newsletters-api-openapi.yml
  format: yaml
  label: Factiva Newsletters API
  slug: factiva-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-factiva-newsletters-api-openapi.yml
- filename: dow-jones-developer-platform-riskcenter-third-party-api-0-2-openapi.yml
  format: yaml
  label: Dow Jones RiskCenter Third Party Platform API
  slug: riskcenter-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-riskcenter-third-party-api-0-2-openapi.yml
auth_types:
- oauth2
- openIdConnect
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Dow Jones Developer Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dow Jones Developer Platform secures its APIs with oauth2, openIdConnect, http, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dow Jones Developer Platform
provider_slug: dow-jones-developer-platform
scheme_count: 4
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dow-jones-developer-platform-calendar-live-api-openapi.yml
  - openapi/dow-jones-developer-platform-company-news-radar-api-openapi.yml
  - openapi/dow-jones-developer-platform-factiva-newsletters-api-openapi.yml
  - openapi/dow-jones-developer-platform-newswires-content-api-openapi.yml
  - openapi/dow-jones-developer-platform-newswires-real-time-api-openapi.yml
  - openapi/dow-jones-developer-platform-newswires-top-stories-api-openapi.yml
  type: http
- in: header
  name: Bearer
  note: Declared as an apiKey header named Authorization; the description in the RiskCenter specs states the value is "bearer {token}".
  parameter: Authorization
  sources:
  - openapi/dow-jones-developer-platform-factiva-content-api-openapi.yml
  - openapi/dow-jones-developer-platform-riskcenter-third-party-api-0-1-openapi.yml
  - openapi/dow-jones-developer-platform-riskcenter-third-party-api-0-2-openapi.yml
  type: apiKey
- in: header
  name: user-key
  note: Legacy per-account key still accepted by the Factiva Analytics endpoints (Streams, Snapshots). Documented in API Essentials and being migrated to OAuth per the OAuth Migration Guide, which states both methods are supported during the transition.
  parameter: user-key
  sources:
  - https://developer.dowjones.com/documents/site-docs-getting_started-api_essentials-getting_a_response
  type: apiKey
- name: FDK session
  note: The Factiva Developer Kit SOAP services authenticate with PerformLogin / PerformEncryptedIDLogin against the Membership service and carry a session id.
  sources:
  - https://developer.dowjones.com/documents/site-docs-factiva_apis-factiva_workflow_apis_soap
  type: soap-session
slug: dow-jones-developer-platform-authentication
source_filename: dow-jones-developer-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://developer.dowjones.com/documents/site-docs-getting_started-sessions_and_authentication\n  (200), https://developer.dowjones.com/documents/site-docs-newswires_apis-oauth-migration-guide (200),\n  https://accounts.dowjones.com/.well-known/openid-configuration (200), plus the securitySchemes of the\n  nine OpenAPI documents in openapi/\ndocs: https://developer.dowjones.com/documents/site-docs-getting_started-sessions_and_authentication\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  primary: OAuth 2.0 bearer token obtained from the Dow Jones Identity Service\n  legacy: A per-account \"user-key\" header is still accepted on the Factiva Analytics endpoints and is\n    being migrated to OAuth\nidentity_service:\n  name: Dow Jones Identity Service\n  issuer: https://sso.accounts.dowjones.com/\n  discovery: https://accounts.dowjones.com/.well-known/openid-configuration\n\
  \  token_endpoint: https://accounts.dowjones.com/oauth2/v1/token\n  authorize_endpoint: https://accounts.dowjones.com/oauth2/v1/authorize\n  logout_endpoint: https://accounts.dowjones.com/oauth2/v1/logout\n  eu_token_endpoint: https://eu.accounts.dowjones.com/oauth2/v1/token\n  riskcenter_third_party_token_endpoint: https://auth-thirdparty.riskcenter.dowjones.com/connect/token\n  jwks_uri: https://sso.accounts.dowjones.com/.well-known/jwks.json\n  registration_endpoint: https://sso.accounts.dowjones.com/register\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:saml2-bearer\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  id_token_signing_alg_values_supported:\n  - HS256\n  -\
  \ RS256\n  flows_documented:\n  - Service Account Integration (server-to-server)\n  - Authorization Code Grant\n  - Implicit Grant\ntoken_exchange:\n  note: 'Dow Jones uses a documented TWO-STEP exchange: the refresh token buys an intermediate access\n    token, which is then presented as a jwt-bearer assertion to obtain the bearer token the APIs accept.\n    An agent that stops after step 1 holds a token that will not authenticate any Dow Jones API call.'\n  steps:\n  - step: 1\n    endpoint: POST https://accounts.dowjones.com/oauth2/v1/token\n    grant_type: refresh_token\n    returns: intermediate access_token\n    lifetime_seconds: 432000\n  - step: 2\n    endpoint: POST https://accounts.dowjones.com/oauth2/v1/token\n    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n    assertion: the intermediate token from step 1\n    scope: openid pib\n    returns: FINAL_ACCESS_TOKEN (Bearer)\n    lifetime_seconds: 3600\n  - step: 3\n    usage: 'Authorization: Bearer <FINAL_ACCESS_TOKEN>\
  \ on every api.dowjones.com request'\n  source: https://developer.dowjones.com/documents/site-docs-newswires_apis-oauth-migration-guide\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/dow-jones-developer-platform-calendar-live-api-openapi.yml\n  - openapi/dow-jones-developer-platform-company-news-radar-api-openapi.yml\n  - openapi/dow-jones-developer-platform-factiva-newsletters-api-openapi.yml\n  - openapi/dow-jones-developer-platform-newswires-content-api-openapi.yml\n  - openapi/dow-jones-developer-platform-newswires-real-time-api-openapi.yml\n  - openapi/dow-jones-developer-platform-newswires-top-stories-api-openapi.yml\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/dow-jones-developer-platform-factiva-content-api-openapi.yml\n  - openapi/dow-jones-developer-platform-riskcenter-third-party-api-0-1-openapi.yml\n  - openapi/dow-jones-developer-platform-riskcenter-third-party-api-0-2-openapi.yml\n\
  \  note: Declared as an apiKey header named Authorization; the description in the RiskCenter specs states\n    the value is \"bearer {token}\".\n- name: user-key\n  type: apiKey\n  in: header\n  parameter: user-key\n  note: Legacy per-account key still accepted by the Factiva Analytics endpoints (Streams, Snapshots).\n    Documented in API Essentials and being migrated to OAuth per the OAuth Migration Guide, which states\n    both methods are supported during the transition.\n  sources:\n  - https://developer.dowjones.com/documents/site-docs-getting_started-api_essentials-getting_a_response\n- name: FDK session\n  type: soap-session\n  note: The Factiva Developer Kit SOAP services authenticate with PerformLogin / PerformEncryptedIDLogin\n    against the Membership service and carry a session id.\n  sources:\n  - https://developer.dowjones.com/documents/site-docs-factiva_apis-factiva_workflow_apis_soap\ncredential_acquisition:\n  self_serve: false\n  note: Credentials are not self-serve.\
  \ Dow Jones documents contacting a representative or submitting\n    the trial-request form.\n  url: https://developer.dowjones.com/request-trial/\n  status: 200\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/authentication/dow-jones-developer-platform-authentication.yml
summary_line: oauth2/openIdConnect/http/apiKey · 4 schemes
tags:
- Business Data
- Compliance
- Financial
- Market Data
- News
- Risk and Compliance
- Screening
- Sanctions
---
