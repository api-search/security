---
api_key_in: []
api_specs:
- filename: kombo-ai-apply-api-openapi.yml
  format: yaml
  label: Kombo AI Apply API
  slug: kombo-ai-apply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-ai-apply-api-openapi.yml
- filename: kombo-custom-endpoints-api-openapi.yml
  format: yaml
  label: Kombo Custom Endpoints API
  slug: kombo-custom-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-custom-endpoints-api-openapi.yml
- filename: kombo-general-api-openapi.yml
  format: yaml
  label: Kombo General API
  slug: kombo-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-general-api-openapi.yml
- filename: kombo-kombo-connect-api-openapi.yml
  format: yaml
  label: Kombo Kombo Connect API
  slug: kombo-kombo-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-kombo-connect-api-openapi.yml
- filename: kombo-unified-ats-api-api-openapi.yml
  format: yaml
  label: Kombo Unified ATS API API
  slug: kombo-unified-ats-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-unified-ats-api-api-openapi.yml
- filename: kombo-unified-ats-assessment-background-check-api-api-openapi.yml
  format: yaml
  label: Kombo Unified ATS (Assessment & Background Check) API API
  slug: kombo-unified-ats-assessment-background-check-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-unified-ats-assessment-background-check-api-api-openapi.yml
- filename: kombo-unified-hris-api-api-openapi.yml
  format: yaml
  label: Kombo Unified HRIS API API
  slug: kombo-unified-hris-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-unified-hris-api-api-openapi.yml
- filename: kombo-unified-lms-api-api-openapi.yml
  format: yaml
  label: Kombo Unified LMS API API
  slug: kombo-unified-lms-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-unified-lms-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kombo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kombo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kombo
provider_slug: kombo
scheme_count: 1
schemes:
- description: Create an API key on the [Secrets](https://app.kombo.dev/secrets) page in the Kombo dashboard.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/kombo-openapi.json
  type: http
slug: kombo-authentication
source_filename: kombo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kombo-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: Create an API key on the [Secrets](https://app.kombo.dev/secrets) page in the\n    Kombo dashboard.\n  sources:\n  - openapi/kombo-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/authentication/kombo-authentication.yml
summary_line: http · 1 scheme
tags:
- ATS
- Embedded iPaaS
- HRIS
- LMS
- Payroll
- Unified-API
---
