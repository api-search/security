---
api_key_in: []
api_specs:
- filename: color-eligibility-openapi.yml
  format: yaml
  label: Color Eligibility List API
  slug: color-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/color/refs/heads/main/openapi/color-eligibility-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Color Authentication
name_suffix: Authentication
oauth_flows: []
overview: Color secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Color
provider_slug: color
scheme_count: 1
schemes:
- description: Per-environment bearer API token in the Authorization header. Obtain separate staging and production tokens from Color.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/color-eligibility-openapi.yml
  type: http
slug: color-authentication
source_filename: color-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.color.com/docs/getting-started-with-color-apis\ndocs: https://docs.color.com/docs/getting-started-with-color-apis\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    API access uses a per-environment bearer API token (static token issued by\n    Color, supplied as Authorization: Bearer <token>). Staging and production\n    each have their own token and base host. Portal/user sign-in is separately\n    handled via SAML 2.0 SSO (see conventions).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Per-environment bearer API token in the Authorization header. Obtain\n    separate staging and production tokens from Color.\n  sources:\n  - openapi/color-eligibility-openapi.yml\nsso:\n  protocol: SAML 2.0\n  idp_initiated: false\n  acs_url: https://colorhealth.kinde.com/login/saml/callback\n  sp_initiated_bookmark: https://home.color.com/start-sso?domain=<email_domain>\n\
  \  docs: https://docs.color.com/docs/sso-integration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/color/refs/heads/main/authentication/color-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Health
- Healthcare
- Genomics
- Oncology
- Cancer Care
- Preventive Health
- Eligibility
- Virtual Care
---
