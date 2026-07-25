---
api_key_in:
- header
api_specs:
- filename: cisco-secure-client-accesspolicies-api-openapi.yml
  format: yaml
  label: Cisco Secure Client AccessPolicies API
  slug: cisco-secure-client-accesspolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/openapi/cisco-secure-client-accesspolicies-api-openapi.yml
- filename: cisco-secure-client-accessrules-api-openapi.yml
  format: yaml
  label: Cisco Secure Client AccessRules API
  slug: cisco-secure-client-accessrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/openapi/cisco-secure-client-accessrules-api-openapi.yml
- filename: cisco-secure-client-authentication-api-openapi.yml
  format: yaml
  label: Cisco Secure Client Authentication API
  slug: cisco-secure-client-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/openapi/cisco-secure-client-authentication-api-openapi.yml
- filename: cisco-secure-client-devices-api-openapi.yml
  format: yaml
  label: Cisco Secure Client Devices API
  slug: cisco-secure-client-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/openapi/cisco-secure-client-devices-api-openapi.yml
- filename: cisco-secure-client-hosts-api-openapi.yml
  format: yaml
  label: Cisco Secure Client Hosts API
  slug: cisco-secure-client-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/openapi/cisco-secure-client-hosts-api-openapi.yml
- filename: cisco-secure-client-networkobjects-api-openapi.yml
  format: yaml
  label: Cisco Secure Client NetworkObjects API
  slug: cisco-secure-client-networkobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/openapi/cisco-secure-client-networkobjects-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Secure Client Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Secure Client secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cisco Secure Client
provider_slug: cisco-secure-client
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/cisco-secure-client-openapi.yml
  type: http
- in: header
  name: tokenAuth
  parameter: X-auth-access-token
  sources:
  - openapi/cisco-secure-client-openapi.yml
  type: apiKey
slug: cisco-secure-client-authentication
source_filename: cisco-secure-client-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-secure-client-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/cisco-secure-client-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-auth-access-token\n  sources:\n  - openapi/cisco-secure-client-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/authentication/cisco-secure-client-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Endpoint Security
- Remote Access
- Security
- VPN
- Zero Trust
---
