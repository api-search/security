---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Synthesized Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synthesized secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synthesized
provider_slug: synthesized
scheme_count: 1
schemes:
- description: Every request to the Governor External API must include a valid access key in the X-Access-Key header. Access keys are created/managed in the Governor application and replaced the deprecated SDK tracking/access tokens (removed in TDK v1.53).
  in: header
  name: AccessKey
  parameter_name: X-Access-Key
  sources:
  - docs
  type: apiKey
slug: synthesized-authentication
source_filename: synthesized-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://docs.synthesized.io/tdk/latest/user_guide/090_cicd/external_api_reference\n  — the Governor External API. Captured from the docs; no downloadable OpenAPI\n  spec is published (the reference is rendered client-side), so this profile is\n  documented rather than derived from a spec file in-repo.\ndocs: https://docs.synthesized.io/tdk/latest/user_guide/090_cicd/external_api_reference\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: AccessKey\n    type: apiKey\n    in: header\n    parameter_name: X-Access-Key\n    description: >-\n      Every request to the Governor External API must include a valid access key\n      in the X-Access-Key header. Access keys are created/managed in the Governor\n      application and replaced the deprecated SDK tracking/access tokens (removed\n      in TDK v1.53).\n    sources: [docs]\nplatform_auth:\n  note: >-\n    Platform-level (Governor\
  \ UI / enterprise) authentication is separate from the\n    External API key. It includes JWT (mandatory JWT secret since v1.41), SAML 2.0\n    SSO, OpenID Connect, LDAP / Active Directory, and Kerberos, with role-based\n    access control (functional + sharing privileges).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthesized/refs/heads/main/authentication/synthesized-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Test Data
- Synthetic Data
- Data Masking
- Data Privacy
- Test Data Management
- Compliance
- Machine Learning
- Databases
- Developer Tools
---
