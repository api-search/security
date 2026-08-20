---
api_key_in:
- header
api_specs:
- filename: safeline-acl-rules-api-openapi.yml
  format: yaml
  label: SafeLine ACL Rules API
  slug: safeline-acl-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-acl-rules-api-openapi.yml
- filename: safeline-authentication-api-openapi.yml
  format: yaml
  label: SafeLine Authentication API
  slug: safeline-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-authentication-api-openapi.yml
- filename: safeline-reports-api-openapi.yml
  format: yaml
  label: SafeLine Reports API
  slug: safeline-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-reports-api-openapi.yml
- filename: safeline-security-policies-api-openapi.yml
  format: yaml
  label: SafeLine Security Policies API
  slug: safeline-security-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-security-policies-api-openapi.yml
- filename: safeline-ssl-certificates-api-openapi.yml
  format: yaml
  label: SafeLine SSL Certificates API
  slug: safeline-ssl-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-ssl-certificates-api-openapi.yml
- filename: safeline-system-api-openapi.yml
  format: yaml
  label: SafeLine System API
  slug: safeline-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-system-api-openapi.yml
- filename: safeline-users-api-openapi.yml
  format: yaml
  label: SafeLine Users API
  slug: safeline-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-users-api-openapi.yml
- filename: safeline-websites-api-openapi.yml
  format: yaml
  label: SafeLine Websites API
  slug: safeline-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/openapi/safeline-websites-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Safeline Authentication
name_suffix: Authentication
oauth_flows: []
overview: SafeLine secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SafeLine
provider_slug: safeline
scheme_count: 1
schemes:
- description: API token obtained from the SafeLine management interface
  in: header
  name: APITokenAuth
  parameter: X-SLCE-API-Token
  sources:
  - openapi/safeline-management-openapi.yml
  type: apiKey
slug: safeline-authentication
source_filename: safeline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/safeline-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APITokenAuth\n  type: apiKey\n  in: header\n  parameter: X-SLCE-API-Token\n  description: API token obtained from the SafeLine management interface\n  sources:\n  - openapi/safeline-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/authentication/safeline-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Proxy
- WAF
- Security
- Open-Source
- Reverse Proxy
- API Gateway
---
