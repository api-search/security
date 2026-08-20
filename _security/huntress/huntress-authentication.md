---
api_key_in: []
api_specs:
- filename: huntress-accounts-api-openapi.yml
  format: yaml
  label: Huntress Accounts API
  slug: huntress-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-accounts-api-openapi.yml
- filename: huntress-actor-api-openapi.yml
  format: yaml
  label: Huntress Actor API
  slug: huntress-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-actor-api-openapi.yml
- filename: huntress-agents-api-openapi.yml
  format: yaml
  label: Huntress Agents API
  slug: huntress-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-agents-api-openapi.yml
- filename: huntress-escalations-api-openapi.yml
  format: yaml
  label: Huntress Escalations API
  slug: huntress-escalations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-escalations-api-openapi.yml
- filename: huntress-external-recon-api-openapi.yml
  format: yaml
  label: Huntress External Recon API
  slug: huntress-external-recon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-external-recon-api-openapi.yml
- filename: huntress-identities-api-openapi.yml
  format: yaml
  label: Huntress Identities API
  slug: huntress-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-identities-api-openapi.yml
- filename: huntress-incident-reports-api-openapi.yml
  format: yaml
  label: Huntress Incident Reports API
  slug: huntress-incident-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-incident-reports-api-openapi.yml
- filename: huntress-invoices-api-openapi.yml
  format: yaml
  label: Huntress Invoices API
  slug: huntress-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-invoices-api-openapi.yml
- filename: huntress-known-vpns-api-openapi.yml
  format: yaml
  label: Huntress Known VPNs API
  slug: huntress-known-vpns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-known-vpns-api-openapi.yml
- filename: huntress-organizations-api-openapi.yml
  format: yaml
  label: Huntress Organizations API
  slug: huntress-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-organizations-api-openapi.yml
- filename: huntress-platform-actions-api-openapi.yml
  format: yaml
  label: Huntress Platform Actions API
  slug: huntress-platform-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-platform-actions-api-openapi.yml
- filename: huntress-reseller-api-openapi.yml
  format: yaml
  label: Huntress Reseller API
  slug: huntress-reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-reseller-api-openapi.yml
- filename: huntress-siem-api-openapi.yml
  format: yaml
  label: Huntress SIEM API
  slug: huntress-siem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-siem-api-openapi.yml
- filename: huntress-signals-api-openapi.yml
  format: yaml
  label: Huntress Signals API
  slug: huntress-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-signals-api-openapi.yml
- filename: huntress-summary-reports-api-openapi.yml
  format: yaml
  label: Huntress Summary Reports API
  slug: huntress-summary-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-summary-reports-api-openapi.yml
- filename: huntress-unwanted-access-rules-api-openapi.yml
  format: yaml
  label: Huntress Unwanted Access Rules API
  slug: huntress-unwanted-access-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-unwanted-access-rules-api-openapi.yml
- filename: huntress-users-api-openapi.yml
  format: yaml
  label: Huntress Users API
  slug: huntress-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Huntress Authentication
name_suffix: Authentication
oauth_flows: []
overview: Huntress secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Huntress
provider_slug: huntress
scheme_count: 1
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/huntress-rest-openapi.json
  type: http
slug: huntress-authentication
source_filename: huntress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/huntress-rest-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/huntress-rest-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/authentication/huntress-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Endpoint Security
- SOC
- SIEM
- Identity Threat Detection
- MSP
- Webhook
---
