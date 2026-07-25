---
api_key_in:
- header
api_specs:
- filename: datadome-account-api-openapi.yml
  format: yaml
  label: DataDome Account API
  slug: datadome-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-account-api-openapi.yml
- filename: datadome-accountprotect-api-openapi.yml
  format: yaml
  label: DataDome AccountProtect API
  slug: datadome-accountprotect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-accountprotect-api-openapi.yml
- filename: datadome-customrules-api-openapi.yml
  format: yaml
  label: DataDome CustomRules API
  slug: datadome-customrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-customrules-api-openapi.yml
- filename: datadome-endpoints-api-openapi.yml
  format: yaml
  label: DataDome Endpoints API
  slug: datadome-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-endpoints-api-openapi.yml
- filename: datadome-priorities-api-openapi.yml
  format: yaml
  label: DataDome Priorities API
  slug: datadome-priorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-priorities-api-openapi.yml
- filename: datadome-templates-api-openapi.yml
  format: yaml
  label: DataDome Templates API
  slug: datadome-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-templates-api-openapi.yml
- filename: datadome-trustedproxies-api-openapi.yml
  format: yaml
  label: DataDome TrustedProxies API
  slug: datadome-trustedproxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-trustedproxies-api-openapi.yml
- filename: datadome-verifiedmodels-api-openapi.yml
  format: yaml
  label: DataDome VerifiedModels API
  slug: datadome-verifiedmodels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-verifiedmodels-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Datadome Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataDome secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataDome
provider_slug: datadome
scheme_count: 1
schemes:
- description: DataDome management API key issued in the customer dashboard.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/datadome-openapi.yml
  type: apiKey
slug: datadome-authentication
source_filename: datadome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datadome-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: DataDome management API key issued in the customer dashboard.\n  sources:\n  - openapi/datadome-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/authentication/datadome-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bot Mitigation
- Fraud Protection
- Account Protection
- Ad Fraud
- DDoS
- Real-Time
- Edge Security
- Application Security
- Agentic Trust
---
