---
api_key_in:
- header
api_specs:
- filename: juniper-networks-apstra-openapi.yml
  format: yaml
  label: Juniper Apstra API
  slug: juniper-apstra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-apstra-openapi.yml
- filename: juniper-networks-junos-telemetry-asyncapi.yml
  format: yaml
  label: Junos XML API
  slug: junos-xml-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/asyncapi/juniper-networks-junos-telemetry-asyncapi.yml
- filename: juniper-networks-mist-openapi.yml
  format: yaml
  label: Juniper Mist API
  slug: juniper-mist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-mist-openapi.yml
- filename: juniper-networks-contrail-openapi.yml
  format: yaml
  label: Juniper Contrail API
  slug: juniper-contrail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-contrail-openapi.yml
- filename: juniper-networks-junos-space-openapi.yml
  format: yaml
  label: Junos Space REST API
  slug: junos-space-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-junos-space-openapi.yml
- filename: juniper-networks-vsrx-openapi.yml
  format: yaml
  label: Juniper vSRX REST API
  slug: juniper-vsrx-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/openapi/juniper-networks-vsrx-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Juniper Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Juniper Networks secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Juniper Networks
provider_slug: juniper-networks
scheme_count: 5
schemes:
- description: Authentication token obtained from POST /api/aaa/login. Include in the AuthToken header for all authenticated API requests.
  in: header
  name: authToken
  parameter: AuthToken
  sources:
  - openapi/juniper-networks-apstra-openapi.yml
  type: apiKey
- description: Keystone authentication token obtained from the OpenStack Identity service. For standalone Contrail, local authentication returns a token via the auth/keystone/v3/auth/tokens endpoint.
  in: header
  name: keystoneToken
  parameter: X-Auth-Token
  sources:
  - openapi/juniper-networks-contrail-openapi.yml
  type: apiKey
- description: HTTP Basic authentication with Junos Space username and password. Also supports X.509 certificate-based authentication.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/juniper-networks-junos-space-openapi.yml
  - openapi/juniper-networks-vsrx-openapi.yml
  type: http
- description: API token authentication. Generate tokens via the Mist dashboard under Organization > Settings > API Token or via POST /self/apitokens. Pass the token in the Authorization header as Bearer {token}.
  name: apiToken
  scheme: bearer
  sources:
  - openapi/juniper-networks-mist-openapi.yml
  type: http
- description: CSRF token for session-based authentication. Obtained from the login response and required for all mutating operations when using cookie authentication.
  in: header
  name: csrfToken
  parameter: X-CSRFToken
  sources:
  - openapi/juniper-networks-mist-openapi.yml
  type: apiKey
slug: juniper-networks-authentication
source_filename: juniper-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/juniper-networks-apstra-openapi.yml, openapi/juniper-networks-contrail-openapi.yml,\n  openapi/juniper-networks-junos-space-openapi.yml, openapi/juniper-networks-mist-openapi.yml,\n  openapi/juniper-networks-vsrx-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: AuthToken\n  description: Authentication token obtained from POST /api/aaa/login. Include in the AuthToken\n    header for all authenticated API requests.\n  sources:\n  - openapi/juniper-networks-apstra-openapi.yml\n- name: keystoneToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Keystone authentication token obtained from the OpenStack Identity service. For\n    standalone Contrail, local authentication returns a token via the auth/keystone/v3/auth/tokens\n    endpoint.\n  sources:\n  - openapi/juniper-networks-contrail-openapi.yml\n\
  - name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with Junos Space username and password. Also supports\n    X.509 certificate-based authentication.\n  sources:\n  - openapi/juniper-networks-junos-space-openapi.yml\n  - openapi/juniper-networks-vsrx-openapi.yml\n- name: apiToken\n  type: http\n  scheme: bearer\n  description: API token authentication. Generate tokens via the Mist dashboard under Organization\n    > Settings > API Token or via POST /self/apitokens. Pass the token in the Authorization\n    header as Bearer {token}.\n  sources:\n  - openapi/juniper-networks-mist-openapi.yml\n- name: csrfToken\n  type: apiKey\n  in: header\n  parameter: X-CSRFToken\n  description: CSRF token for session-based authentication. Obtained from the login response\n    and required for all mutating operations when using cookie authentication.\n  sources:\n  - openapi/juniper-networks-mist-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/authentication/juniper-networks-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Automation
- Cloud
- Data Center
- Enterprise
- Networking
- SDN
- Security
- Fortune 1000
---
