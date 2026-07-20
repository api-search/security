---
api_key_in:
- header
api_specs:
- filename: api-explorer
  format: yaml
  label: Junos Space API
  slug: junos-space-api
  spec_type: OpenAPI
  url: https://[space-server]/api/space/api-explorer
- filename: juniper-apstra-openapi.yml
  format: yaml
  label: Juniper Apstra API
  slug: juniper-apstra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/openapi/juniper-apstra-openapi.yml
- filename: juniper-junos-rest-api-openapi.yml
  format: yaml
  label: Junos REST API
  slug: junos-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/openapi/juniper-junos-rest-api-openapi.yml
- filename: docs
  format: yaml
  label: Juniper Mist API
  slug: juniper-mist-api
  spec_type: OpenAPI
  url: https://api.mist.com/api/v1/docs
- filename: juniper-contrail-openapi.yml
  format: yaml
  label: Contrail Networking API
  slug: contrail-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/openapi/juniper-contrail-openapi.yml
- filename: juniper-atp-cloud-openapi.yml
  format: yaml
  label: Juniper ATP Cloud API
  slug: juniper-atp-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/openapi/juniper-atp-cloud-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Juniper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Juniper Networks secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Juniper Networks
provider_slug: juniper
scheme_count: 5
schemes:
- description: Authentication token obtained from the /aaa/login endpoint. Include as AuthToken header in all requests.
  in: header
  name: authToken
  parameter: AuthToken
  sources:
  - openapi/juniper-apstra-openapi.yml
  type: apiKey
- description: API token obtained from the login endpoint
  in: header
  name: apiKey
  parameter: X-Auth-Token
  sources:
  - openapi/juniper-atp-cloud-openapi.yml
  type: apiKey
- description: Keystone token authentication. Obtain a token from the Keystone identity service and pass it as X-Auth-Token header.
  name: keystoneAuth
  scheme: bearer
  sources:
  - openapi/juniper-contrail-openapi.yml
  - openapi/juniper-mist-openapi.yml
  type: http
- description: HTTP Basic authentication with Junos device credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/juniper-junos-rest-api-openapi.yml
  - openapi/juniper-junos-space-openapi.yml
  type: http
- description: CSRF token for session-based authentication.
  in: header
  name: csrfToken
  parameter: X-CSRFToken
  sources:
  - openapi/juniper-mist-openapi.yml
  type: apiKey
slug: juniper-authentication
source_filename: juniper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/juniper-apstra-openapi.yml, openapi/juniper-atp-cloud-openapi.yml, openapi/juniper-contrail-openapi.yml,\n  openapi/juniper-junos-rest-api-openapi.yml, openapi/juniper-junos-space-openapi.yml, openapi/juniper-mist-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: AuthToken\n  description: Authentication token obtained from the /aaa/login endpoint. Include as AuthToken\n    header in all requests.\n  sources:\n  - openapi/juniper-apstra-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: API token obtained from the login endpoint\n  sources:\n  - openapi/juniper-atp-cloud-openapi.yml\n- name: keystoneAuth\n  type: http\n  scheme: bearer\n  description: Keystone token authentication. Obtain a token from the Keystone identity service\n    and pass it as X-Auth-Token header.\n\
  \  sources:\n  - openapi/juniper-contrail-openapi.yml\n  - openapi/juniper-mist-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with Junos device credentials\n  sources:\n  - openapi/juniper-junos-rest-api-openapi.yml\n  - openapi/juniper-junos-space-openapi.yml\n- name: csrfToken\n  type: apiKey\n  in: header\n  parameter: X-CSRFToken\n  description: CSRF token for session-based authentication.\n  sources:\n  - openapi/juniper-mist-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/authentication/juniper-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- AI
- Automation
- Cloud
- Enterprise
- Networking
- SDN
- Security
- Fortune 1000
---
