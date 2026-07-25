---
api_key_in:
- header
api_specs:
- filename: upguard-breaches-api-openapi.yml
  format: yaml
  label: UpGuard breaches API
  slug: upguard-breaches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-breaches-api-openapi.yml
- filename: upguard-bulk-api-openapi.yml
  format: yaml
  label: UpGuard bulk API
  slug: upguard-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-bulk-api-openapi.yml
- filename: upguard-dataleaks-api-openapi.yml
  format: yaml
  label: UpGuard dataleaks API
  slug: upguard-dataleaks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-dataleaks-api-openapi.yml
- filename: upguard-domains-api-openapi.yml
  format: yaml
  label: UpGuard domains API
  slug: upguard-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-domains-api-openapi.yml
- filename: upguard-ips-api-openapi.yml
  format: yaml
  label: UpGuard ips API
  slug: upguard-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-ips-api-openapi.yml
- filename: upguard-labels-api-openapi.yml
  format: yaml
  label: UpGuard labels API
  slug: upguard-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-labels-api-openapi.yml
- filename: upguard-notifications-api-openapi.yml
  format: yaml
  label: UpGuard notifications API
  slug: upguard-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-notifications-api-openapi.yml
- filename: upguard-organisation-api-openapi.yml
  format: yaml
  label: UpGuard organisation API
  slug: upguard-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-organisation-api-openapi.yml
- filename: upguard-reports-api-openapi.yml
  format: yaml
  label: UpGuard reports API
  slug: upguard-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-reports-api-openapi.yml
- filename: upguard-risks-api-openapi.yml
  format: yaml
  label: UpGuard risks API
  slug: upguard-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-risks-api-openapi.yml
- filename: upguard-subsidiaries-api-openapi.yml
  format: yaml
  label: UpGuard subsidiaries API
  slug: upguard-subsidiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-subsidiaries-api-openapi.yml
- filename: upguard-threatmonitoring-api-openapi.yml
  format: yaml
  label: UpGuard threatmonitoring API
  slug: upguard-threatmonitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-threatmonitoring-api-openapi.yml
- filename: upguard-trust-exchange-api-openapi.yml
  format: yaml
  label: UpGuard trust_exchange API
  slug: upguard-trust-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-trust-exchange-api-openapi.yml
- filename: upguard-typosquat-api-openapi.yml
  format: yaml
  label: UpGuard typosquat API
  slug: upguard-typosquat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-typosquat-api-openapi.yml
- filename: upguard-userrisk-api-openapi.yml
  format: yaml
  label: UpGuard userrisk API
  slug: upguard-userrisk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-userrisk-api-openapi.yml
- filename: upguard-vendors-api-openapi.yml
  format: yaml
  label: UpGuard vendors API
  slug: upguard-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-vendors-api-openapi.yml
- filename: upguard-vulnerabilities-api-openapi.yml
  format: yaml
  label: UpGuard vulnerabilities API
  slug: upguard-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-vulnerabilities-api-openapi.yml
- filename: upguard-webhooks-api-openapi.yml
  format: yaml
  label: UpGuard webhooks API
  slug: upguard-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Upguard Authentication
name_suffix: Authentication
oauth_flows: []
overview: UpGuard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UpGuard
provider_slug: upguard
scheme_count: 1
schemes:
- in: header
  name: API key in header
  parameter: Authorization
  sources:
  - openapi/upguard-cyberrisk-openapi-original.json
  type: apiKey
slug: upguard-authentication
source_filename: upguard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/upguard-cyberrisk-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API key in header\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/upguard-cyberrisk-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/authentication/upguard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Third-Party Risk Management
- Attack Surface Management
- Vendor Risk
- Security Ratings
- Data Leaks
- Threat Intelligence
---
