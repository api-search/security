---
api_key_in:
- cookie
api_specs:
- filename: genialis-base-openapi.yaml
  format: yaml
  label: Genialis Expressions API
  slug: genialis-expressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genialis/refs/heads/main/openapi/genialis-base-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Genialis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genialis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Genialis
provider_slug: genialis
scheme_count: 1
schemes:
- in: cookie
  name: cookieAuth
  note: The only security scheme in the contract. Applied per-operation; there is no global `security` block. Several operations declare `[cookieAuth, {}]`, i.e. anonymous access is explicitly permitted.
  parameter: sessionid
  sources:
  - openapi/genialis-base-openapi.yaml
  type: apiKey
slug: genialis-authentication
source_filename: genialis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: searched\nsource: >-\n  openapi/genialis-base-openapi.yaml (securitySchemes + the /rest-auth and\n  /saml-auth operations), https://docs.genialis.com/resdk/start.html (the documented\n  login flow), and the OIDC discovery document at\n  https://genialis.us.auth0.com/.well-known/openid-configuration probed 2026-08-21\ndocs: https://docs.genialis.com/resdk/start.html\napi: Genialis Expressions API\nbase_url: https://app.genialis.com\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  bearer_token: false\n  api_key_header: false\n  oauth2_for_api: false\n  scopes: false\n  federated_login: true\n  sso: saml\n  anonymous_read: true\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/genialis-base-openapi.yaml\n  note: >-\n    The only security scheme in the contract. Applied per-operation; there is no\n    global `security` block. Several operations declare `[cookieAuth, {}]`, i.e.\n\
  \    anonymous access is explicitly permitted.\nanonymous_access:\n  supported: true\n  evidence:\n  - request: GET https://app.genialis.com/api/data?limit=1\n    status: 200\n    note: 'returned {\"count\":29123,...} with no credentials'\n  - request: GET https://app.genialis.com/api/collection?limit=1\n    status: 200\n    note: 'returned {\"count\":107,...}'\n  - request: GET https://app.genialis.com/api/user\n    status: 200\n    note: 'returned [] — anonymous sees no users'\n  scope: Public and community datasets only. Private objects require a session.\nidentity_provider:\n  vendor: Auth0\n  tenant: https://genialis.us.auth0.com/\n  discovery: https://genialis.us.auth0.com/.well-known/openid-configuration\n  discovery_status: 200\n  saved: well-known/genialis-openid-configuration.json\n  protocols: [OIDC, OAuth 2.0]\n  pkce: S256\n  id_token_algs: [RS256, HS256, PS256]\n  idp_scopes: [openid, profile, email, offline_access, phone, address]\n  important: >-\n    These are the IdP's\
  \ OIDC scopes, NOT API authorization scopes. The Genialis REST\n    API does not accept an Auth0 access token — the browser flow terminates in a\n    Django `sessionid` cookie, and that cookie is what the API reads. There is no\n    scope model for API resources; authorization is per-object ACL (see\n    data-model/genialis-data-model.yml, permissions_model).\n  how_found: >-\n    The restricted docs.genialis.com sections (supermodel, gpm, deploy, internal)\n    302 to https://genialis.us.auth0.com/u/login.\nflows:\n- id: resdk-interactive\n  documented: true\n  docs: https://docs.genialis.com/resdk/start.html\n  headless: false\n  code: |\n    import resdk\n    res = resdk.Resolwe(url='https://app.genialis.com')\n    res.login()          # performs interactive login in a web browser\n    resdk.start_logging()\n  note: >-\n    The only flow Genialis documents. Quoted from the docs: \"The `login()` call will\n    perform interactive login in a web browser\" and \"If you omit the `login()`\
  \ line\n    you will be logged as anonymous user.\" An unattended agent cannot complete this\n    without a human at a browser.\n- id: rest-auth-session\n  documented: false\n  operations:\n  - id: rest_auth_login_create\n    method: POST\n    path: /rest-auth/login/\n    description: Attempt to perform automatic login.\n  - id: rest_auth_logout_create\n    method: POST\n    path: /rest-auth/logout/\n    description: Calls Django logout method and deletes the Token object assigned to the user.\n  - id: rest_auth_user_retrieve\n    method: GET\n    path: /rest-auth/user/\n    description: Reads and updates UserModel fields.\n    use: cheapest way to verify a live session\n  - id: rest_auth_password_change_create\n    method: POST\n    path: /rest-auth/password/change/\n  - id: rest_auth_password_reset_create\n    method: POST\n    path: /rest-auth/password/reset/\n  - id: rest_auth_password_reset_confirm_create\n    method: POST\n    path: /rest-auth/password/reset/confirm/\n  gap: >-\n\
  \    django-rest-auth endpoints are present in the contract but declare NO request\n    body schema and NO error responses, so the credential field names are not\n    discoverable from the spec and no failure mode is described.\n- id: saml-sso\n  documented: false\n  operations:\n  - id: saml_auth_api_login_create\n    method: POST\n    path: /saml-auth/api-login/\n    description: Attempt to perform automatic login.\n  - id: saml_auth_remote_login_auth_id_retrieve\n    method: GET\n    path: /saml-auth/remote-login/auth-id/\n    description: Generate a cryptographically secure auth_id token.\n  - id: saml_auth_remote_login_poll_retrieve\n    method: GET\n    path: /saml-auth/remote-login/poll/\n    description: Poll the redis server for authentication data.\n  note: >-\n    A device-style pairing flow — mint an auth_id, send the user to the IdP, poll\n    until the session materialises. This is the mechanism behind resdk's browser\n    login and it is the enterprise SSO surface.\nauthorization:\n\
  \  model: per-object ACL\n  endpoints:\n  - /api/data/{id}/permissions\n  - /api/collection/{id}/permissions\n  - /api/sample/{id}/permissions\n  - /api/process/{id}/permissions\n  - /api/descriptorschema/{id}/permissions\n  principals: [user, group, public]\n  scopes: none\noutbound_oauth:\n  note: >-\n    Genialis acts as an OAuth CLIENT against Illumina BaseSpace:\n    /api/basespace/oauth_browse_url and /api/basespace/oauth_read_projects_url return\n    URLs for requesting BaseSpace permissions. This is not inbound API auth.\ngaps:\n- No machine-to-machine credential. There is no API key, no bearer token and no client_credentials path to the REST API — every documented route to a session requires a human at a browser.\n- No 401/403 response is documented on any of the 254 operations.\n- The /rest-auth/* operations have no request schema, so the login payload cannot be built from the contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genialis/refs/heads/main/authentication/genialis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Bioinformatics
- Precision Medicine
- Genomics
- Life Sciences
- Healthcare
- Machine Learning
- Artificial Intelligence
- Multiomics
- Oncology
- Data Platform
- Open Source
---
