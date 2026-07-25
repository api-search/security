---
api_key_in: []
api_specs:
- filename: onetrust-ai-governance-api-openapi.yml
  format: yaml
  label: OneTrust AI Governance API
  slug: onetrust-ai-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/openapi/onetrust-ai-governance-api-openapi.yml
- filename: onetrust-applications-api-openapi.yml
  format: yaml
  label: OneTrust Applications API
  slug: onetrust-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/openapi/onetrust-applications-api-openapi.yml
- filename: onetrust-consent-api-openapi.yml
  format: yaml
  label: OneTrust Consent API
  slug: onetrust-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/openapi/onetrust-consent-api-openapi.yml
- filename: onetrust-cookies-api-openapi.yml
  format: yaml
  label: OneTrust Cookies API
  slug: onetrust-cookies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/openapi/onetrust-cookies-api-openapi.yml
- filename: onetrust-data-subjects-api-openapi.yml
  format: yaml
  label: OneTrust Data Subjects API
  slug: onetrust-data-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/openapi/onetrust-data-subjects-api-openapi.yml
- filename: onetrust-domains-api-openapi.yml
  format: yaml
  label: OneTrust Domains API
  slug: onetrust-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/openapi/onetrust-domains-api-openapi.yml
- filename: onetrust-privacy-notices-api-openapi.yml
  format: yaml
  label: OneTrust Privacy Notices API
  slug: onetrust-privacy-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/openapi/onetrust-privacy-notices-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Onetrust Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneTrust secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OneTrust
provider_slug: onetrust
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT bearer token issued via OAuth 2.0 client credentials.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/onetrust-openapi.yml
  type: http
slug: onetrust-authentication
source_filename: onetrust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/onetrust-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token issued via OAuth 2.0 client credentials.\n  sources:\n  - openapi/onetrust-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/authentication/onetrust-authentication.yml
summary_line: http · 1 scheme
tags:
- Privacy
- GRC
- Compliance
- Consent
- TPRM
---
