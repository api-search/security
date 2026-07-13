---
api_key_in:
- header
api_specs:
- filename: f5-distributed-cloud-services-openapi.yml
  format: yaml
  label: F5 Distributed Cloud Services API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-distributed-cloud-services/refs/heads/main/openapi/f5-distributed-cloud-services-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: F5 Distributed Cloud Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: F5 Distributed Cloud Services secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: F5 Distributed Cloud Services
provider_slug: f5-distributed-cloud-services
scheme_count: 1
schemes:
- description: 'Send "Authorization: APIToken {token}" using a token issued from

    the F5 Distributed Cloud Console (Personal Tokens or Service

    Credentials).'
  in: header
  name: APIToken
  parameter: Authorization
  sources:
  - openapi/f5-distributed-cloud-services-openapi.yml
  type: apiKey
slug: f5-distributed-cloud-services-authentication
source_filename: f5-distributed-cloud-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/f5-distributed-cloud-services-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Send \"Authorization: APIToken {token}\" using a token issued from\n    the F5 Distributed Cloud Console (Personal Tokens or Service\n    Credentials).\n  sources:\n  - openapi/f5-distributed-cloud-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5-distributed-cloud-services/refs/heads/main/authentication/f5-distributed-cloud-services-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Security
- Web Application Firewall
- API Security
- Multi-Cloud Networking
- DDoS Protection
- Bot Defense
- Load Balancing
- Edge Compute
---
