---
api_key_in: []
api_specs:
- filename: root-applications-api-openapi.yml
  format: yaml
  label: Root Insurance Applications API
  slug: root-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-applications-api-openapi.yml
- filename: root-calls-api-openapi.yml
  format: yaml
  label: Root Insurance Calls API
  slug: root-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-calls-api-openapi.yml
- filename: root-claims-api-openapi.yml
  format: yaml
  label: Root Insurance Claims API
  slug: root-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-claims-api-openapi.yml
- filename: root-complaints-api-openapi.yml
  format: yaml
  label: Root Insurance Complaints API
  slug: root-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-complaints-api-openapi.yml
- filename: root-data-exports-api-openapi.yml
  format: yaml
  label: Root Insurance Data exports API
  slug: root-data-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-data-exports-api-openapi.yml
- filename: root-data-stores-api-openapi.yml
  format: yaml
  label: Root Insurance Data stores API
  slug: root-data-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-data-stores-api-openapi.yml
- filename: root-embed-api-openapi.yml
  format: yaml
  label: Root Insurance Embed API
  slug: root-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-embed-api-openapi.yml
- filename: root-files-api-openapi.yml
  format: yaml
  label: Root Insurance Files API
  slug: root-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-files-api-openapi.yml
- filename: root-leads-api-openapi.yml
  format: yaml
  label: Root Insurance Leads API
  slug: root-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-leads-api-openapi.yml
- filename: root-notifications-api-openapi.yml
  format: yaml
  label: Root Insurance Notifications API
  slug: root-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-notifications-api-openapi.yml
- filename: root-payment-methods-api-openapi.yml
  format: yaml
  label: Root Insurance Payment Methods API
  slug: root-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-payment-methods-api-openapi.yml
- filename: root-payments-api-openapi.yml
  format: yaml
  label: Root Insurance Payments API
  slug: root-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-payments-api-openapi.yml
- filename: root-policies-api-openapi.yml
  format: yaml
  label: Root Insurance Policies API
  slug: root-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-policies-api-openapi.yml
- filename: root-policyholders-api-openapi.yml
  format: yaml
  label: Root Insurance Policyholders API
  slug: root-policyholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-policyholders-api-openapi.yml
- filename: root-quotes-api-openapi.yml
  format: yaml
  label: Root Insurance Quotes API
  slug: root-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-quotes-api-openapi.yml
- filename: root-secret-keys-api-openapi.yml
  format: yaml
  label: Root Insurance Secret keys API
  slug: root-secret-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-secret-keys-api-openapi.yml
- filename: root-webhooks-api-openapi.yml
  format: yaml
  label: Root Insurance Webhooks API
  slug: root-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/openapi/root-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Root Authentication
name_suffix: Authentication
oauth_flows: []
overview: Root Insurance secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Root Insurance
provider_slug: root
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/root-platform-api-openapi.json
  type: http
slug: root-authentication
source_filename: root-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/root-platform-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/root-platform-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/authentication/root-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Auto Insurance
- Telematics
- Embedded Insurance
- Policy Administration
- Claims
- Usage-Based Insurance
- Insurtech
---
