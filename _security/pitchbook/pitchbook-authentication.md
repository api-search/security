---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: pitchbook-account-information-api-openapi.yml
  format: yaml
  label: PitchBook Account Information API
  slug: pitchbook-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-account-information-api-openapi.yml
- filename: pitchbook-companies-api-openapi.yml
  format: yaml
  label: PitchBook Companies API
  slug: pitchbook-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-companies-api-openapi.yml
- filename: pitchbook-credit-analysis-api-openapi.yml
  format: yaml
  label: PitchBook Credit Analysis API
  slug: pitchbook-credit-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-credit-analysis-api-openapi.yml
- filename: pitchbook-deals-api-openapi.yml
  format: yaml
  label: PitchBook Deals API
  slug: pitchbook-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-deals-api-openapi.yml
- filename: pitchbook-fundamentals-api-openapi.yml
  format: yaml
  label: PitchBook Fundamentals API
  slug: pitchbook-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-fundamentals-api-openapi.yml
- filename: pitchbook-funds-api-openapi.yml
  format: yaml
  label: PitchBook Funds API
  slug: pitchbook-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-funds-api-openapi.yml
- filename: pitchbook-general-api-openapi.yml
  format: yaml
  label: PitchBook General API
  slug: pitchbook-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-general-api-openapi.yml
- filename: pitchbook-investors-api-openapi.yml
  format: yaml
  label: PitchBook Investors API
  slug: pitchbook-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-investors-api-openapi.yml
- filename: pitchbook-limited-partners-api-openapi.yml
  format: yaml
  label: PitchBook Limited Partners API
  slug: pitchbook-limited-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-limited-partners-api-openapi.yml
- filename: pitchbook-patents-api-openapi.yml
  format: yaml
  label: PitchBook Patents API
  slug: pitchbook-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-patents-api-openapi.yml
- filename: pitchbook-people-api-openapi.yml
  format: yaml
  label: PitchBook People API
  slug: pitchbook-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-people-api-openapi.yml
- filename: pitchbook-service-providers-api-openapi.yml
  format: yaml
  label: PitchBook Service Providers API
  slug: pitchbook-service-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/openapi/pitchbook-service-providers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Pitchbook Authentication
name_suffix: Authentication
oauth_flows: []
overview: PitchBook secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PitchBook
provider_slug: pitchbook
scheme_count: 1
schemes:
- in: header
  name: pbToken
  parameter: Authorization
  sources:
  - openapi/pitchbook-openapi.json
  type: apiKey
slug: pitchbook-authentication
source_filename: pitchbook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: derived\nsource: openapi/pitchbook-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: pbToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/pitchbook-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pitchbook/refs/heads/main/authentication/pitchbook-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- Finance
- Private-Market
- Analytics
---
