---
api_key_in:
- header
api_specs:
- filename: proctorio-openapi.yml
  format: yaml
  label: Proctorio Launch API (v2)
  slug: proctorio-launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proctorio/refs/heads/main/openapi/proctorio-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Proctorio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proctorio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Proctorio
provider_slug: proctorio
scheme_count: 1
schemes:
- description: OAuth-style HMAC signature computed from the Proctorio-provisioned consumer key and secret. In the official .NET client this is produced by Helpers.GetApiKey(consumerKey, consumerSecret) and attached to the request; the GetCertified/TAO integrations describe HMAC-SHA1 signing.
  in: header
  name: proctorioHmac
  parameter: Authorization
  sources:
  - openapi/proctorio-openapi.yml
  type: apiKey
slug: proctorio-authentication
source_filename: proctorio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/proctorio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: proctorioHmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: OAuth-style HMAC signature computed from the Proctorio-provisioned consumer key\n    and secret. In the official .NET client this is produced by Helpers.GetApiKey(consumerKey,\n    consumerSecret) and attached to the request; the GetCertified/TAO integrations describe\n    HMAC-SHA1 signing.\n  sources:\n  - openapi/proctorio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proctorio/refs/heads/main/authentication/proctorio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Online Proctoring
- Remote Proctoring
- Exam Integrity
- Assessment
- EdTech
- LTI
- LMS Integration
- Learning Integrity
---
