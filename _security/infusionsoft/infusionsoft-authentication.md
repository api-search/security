---
api_key_in: []
api_specs:
- filename: infusionsoft-rest-v2-openapi.json
  format: json
  label: Keap REST API v2
  slug: rest-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/openapi/infusionsoft-rest-v2-openapi.json
- filename: infusionsoft-rest-v1-openapi.json
  format: json
  label: Keap REST API v1
  slug: rest-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/openapi/infusionsoft-rest-v1-openapi.json
- filename: infusionsoft-pipelines-openapi.yml
  format: yaml
  label: Keap Pipelines API
  slug: pipelines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/openapi/infusionsoft-pipelines-openapi.yml
auth_types:
- oauth2
- bearer
description: ''
kind: authentication
layout: security
method: searched
name: Infusionsoft Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Infusionsoft (Keap) secures its APIs with oauth2 and bearer across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Infusionsoft (Keap)
provider_slug: infusionsoft
scheme_count: 3
schemes:
- access_token_lifetime: communicated per-response in expires_in; no fixed value published
  authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize
  authorize_params:
    client_id: from the developer portal at https://keys.developer.keap.com
    redirect_uri: must be HTTPS
    response_type: code
    scope: full (the only valid value)
  flow: authorizationCode
  name: oauth2
  presentation: 'Authorization: Bearer <access_token>'
  refresh:
    note: Each refresh returns a NEW refresh token; the old one is discarded and the new one must be persisted or the integration will lock itself out.
    rotating: true
    supported: true
  sources:
  - openapi/infusionsoft-rest-v1-openapi.json
  - openapi/infusionsoft-rest-v2-openapi.json
  - openapi/infusionsoft-pipelines-openapi.yml
  - https://developer.keap.com/getting-started-oauth-keys/
  tokenUrl: https://api.infusionsoft.com/token
  token_endpoint_auth: HTTP Basic - base64(client_id:client_secret)
  token_request: POST application/x-www-form-urlencoded with client_id, client_secret, code, grant_type=authorization_code, redirect_uri
  type: oauth2
- created_by: any app user, from API Settings (Settings menu in Keap, Profile menu in Keap Classic)
  expiry: none published
  name: Personal Access Token (PAT)
  permission_model: runs under the creating user context, with that user visibility and editing permissions
  prefix: null
  presentation: 'Authorization: Bearer <token>'
  rate_limits: 10/sec, 240/min, 30,000/day per key
  revocation: delete the key in API Settings
  scheme: bearer
  scope: a single Keap application
  source: https://developer.keap.com/pat-and-sak/
  type: http
- created_by: administrators only
  expiry: none published
  name: Service Account Key (SAK)
  permission_model: admin access to ALL stored data in the application - there is no way to narrow it
  prefix: null
  presentation: 'Authorization: Bearer <token>'
  rate_limits: 10/sec, 240/min, 30,000/day per key
  scheme: bearer
  scope: a single Keap application
  source: https://developer.keap.com/pat-and-sak/
  type: http
slug: infusionsoft-authentication
source_filename: infusionsoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.keap.com/getting-started-oauth-keys/, https://developer.keap.com/pat-and-sak/,\n  https://developer.keap.com/faqs/can-use-api-key/, openapi/infusionsoft-rest-v1-openapi.json, openapi/infusionsoft-rest-v2-openapi.json,\n  openapi/infusionsoft-pipelines-openapi.yml\ndocs: https://developer.keap.com/getting-started-oauth-keys/\nnote: 'The OpenAPI under-describes Keap authentication. All three specs declare only an oauth2 authorizationCode\n  scheme, but Keap actually supports THREE credential types in production: OAuth 2.0 user-authorized tokens,\n  Personal Access Tokens, and Service Account Keys. All three are presented identically as `Authorization:\n  Bearer <token>`, so a server cannot tell them apart from the header - only the rate limits and the permission\n  model differ. Legacy Infusionsoft API keys are retired and no longer accepted. The Pipelines spec is\n  the only one that names a second scheme (BearerAuth)\
  \ alongside oauth2.'\nsummary:\n  types:\n  - oauth2\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  credential_types: 3\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize\n  tokenUrl: https://api.infusionsoft.com/token\n  token_endpoint_auth: HTTP Basic - base64(client_id:client_secret)\n  authorize_params:\n    client_id: from the developer portal at https://keys.developer.keap.com\n    redirect_uri: must be HTTPS\n    response_type: code\n    scope: full (the only valid value)\n  token_request: POST application/x-www-form-urlencoded with client_id, client_secret, code, grant_type=authorization_code,\n    redirect_uri\n  refresh:\n    supported: true\n    rotating: true\n    note: Each refresh returns a NEW refresh token; the old one is discarded and the new one must be persisted\n      or the integration will lock itself out.\n  access_token_lifetime: communicated per-response in expires_in;\
  \ no fixed value published\n  presentation: 'Authorization: Bearer <access_token>'\n  sources:\n  - openapi/infusionsoft-rest-v1-openapi.json\n  - openapi/infusionsoft-rest-v2-openapi.json\n  - openapi/infusionsoft-pipelines-openapi.yml\n  - https://developer.keap.com/getting-started-oauth-keys/\n- name: Personal Access Token (PAT)\n  type: http\n  scheme: bearer\n  presentation: 'Authorization: Bearer <token>'\n  prefix: null\n  created_by: any app user, from API Settings (Settings menu in Keap, Profile menu in Keap Classic)\n  permission_model: runs under the creating user context, with that user visibility and editing permissions\n  scope: a single Keap application\n  expiry: none published\n  revocation: delete the key in API Settings\n  rate_limits: 10/sec, 240/min, 30,000/day per key\n  source: https://developer.keap.com/pat-and-sak/\n- name: Service Account Key (SAK)\n  type: http\n  scheme: bearer\n  presentation: 'Authorization: Bearer <token>'\n  prefix: null\n  created_by: administrators\
  \ only\n  permission_model: admin access to ALL stored data in the application - there is no way to narrow it\n  scope: a single Keap application\n  expiry: none published\n  rate_limits: 10/sec, 240/min, 30,000/day per key\n  source: https://developer.keap.com/pat-and-sak/\nretired:\n- name: Legacy Infusionsoft API key\n  status: retired\n  note: Keap states API keys are no longer supported and OAuth 2.0 (or PAT/SAK) is mandatory - https://developer.keap.com/faqs/can-use-api-key/\nscopes:\n  granular: false\n  see: scopes/infusionsoft-scopes.yml\nmtls: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/authentication/infusionsoft-authentication.yml
summary_line: oauth2/bearer · 3 schemes
tags:
- CRM
- Marketing Automation
- Sales Automation
- Email Marketing
- E-Commerce
- Small Business
- Contacts
- Subscription
- Webhook
- Authentication
---
