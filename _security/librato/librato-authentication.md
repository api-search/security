---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Librato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Librato secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Librato
provider_slug: librato
scheme_count: 1
schemes:
- credential_password: API token
  credential_user: account email address
  description: HTTP Basic authentication is required on every request. The username is the email address used to create the Librato Metrics account; the password is an API token issued from the account tokens page. All requests must be sent over HTTPS — a plaintext request is rejected with 403 and the error message "Please use secured connection through https!".
  name: basicAuth
  scheme: basic
  sources:
  - https://github.com/librato/api-docs/blob/master/source/includes/_authentication.md
  token_management: https://metrics.librato.com/tokens
  type: http
slug: librato-authentication
source_filename: librato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/librato/api-docs/blob/master/source/includes/_authentication.md\ndocs: https://github.com/librato/api-docs/blob/master/source/includes/_authentication.md\nstatus: retired\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  transport: https-only\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic authentication is required on every request. The username is the\n    email address used to create the Librato Metrics account; the password is an API token\n    issued from the account tokens page. All requests must be sent over HTTPS — a plaintext\n    request is rejected with 403 and the error message \"Please use secured connection\n    through https!\".'\n  credential_user: account email address\n  credential_password: API token\n  token_management: https://metrics.librato.com/tokens\n  sources:\n  - https://github.com/librato/api-docs/blob/master/source/includes/_authentication.md\n\
  notes:\n- Credentials may alternatively be embedded in the URL (https://user:token@metrics-api.librato.com/v1/metrics);\n  because the user is an email address the \"@\" must be percent-encoded as %40.\n- 'API tokens are themselves managed through the API: the /v1/api_tokens resource supports\n  create, retrieve, update, delete and list.'\n- No OAuth 2.0, OpenID Connect, mTLS or scoped-permission surface was ever documented for\n  this API, so no scopes/ artifact applies.\n- The authenticating host metrics-api.librato.com no longer resolves; this profile is a\n  historical record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/librato/refs/heads/main/authentication/librato-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Monitoring
- Metrics
- Observability
- Time Series
- Alerting
- Dashboards
- Analytics
- Retired
---
