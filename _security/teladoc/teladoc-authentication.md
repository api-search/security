---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Teladoc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teladoc secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Teladoc
provider_slug: teladoc
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter_name: Api-Key
  sources:
  - https://intouchhealth.github.io/solo-slate/
  type: apiKey
slug: teladoc-authentication
source_filename: teladoc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://intouchhealth.github.io/solo-slate/\ndocs: https://intouchhealth.github.io/solo-slate/\napi: Teladoc Health Solo External API\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    The Solo External API authenticates every request with a static API key\n    passed in the Api-Key request header. Keys are issued per practice/tenant by\n    Teladoc Health. Access to the API and SDK documentation is granted on request\n    (partners email Teladoc Health). No OAuth2/OIDC surface is documented; the API\n    is machine-to-machine with a Business Associate Agreement (BAA) required for\n    handling PHI.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: Api-Key\n  sources:\n  - https://intouchhealth.github.io/solo-slate/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teladoc/refs/heads/main/authentication/teladoc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Healthtech
- Telehealth
- Telemedicine
- Virtual Care
- Healthcare
- Behavioral Health
- Webhooks
- API
---
