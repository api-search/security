---
api_key_in:
- header
api_specs:
- filename: tutorcruncher-agents-api-openapi.yml
  format: yaml
  label: TutorCruncher Agents API
  slug: tutorcruncher-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-agents-api-openapi.yml
- filename: tutorcruncher-appointments-api-openapi.yml
  format: yaml
  label: TutorCruncher Appointments API
  slug: tutorcruncher-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-appointments-api-openapi.yml
- filename: tutorcruncher-clients-api-openapi.yml
  format: yaml
  label: TutorCruncher Clients API
  slug: tutorcruncher-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-clients-api-openapi.yml
- filename: tutorcruncher-contractors-api-openapi.yml
  format: yaml
  label: TutorCruncher Contractors API
  slug: tutorcruncher-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-contractors-api-openapi.yml
- filename: tutorcruncher-invoices-api-openapi.yml
  format: yaml
  label: TutorCruncher Invoices API
  slug: tutorcruncher-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-invoices-api-openapi.yml
- filename: tutorcruncher-payments-api-openapi.yml
  format: yaml
  label: TutorCruncher Payments API
  slug: tutorcruncher-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-payments-api-openapi.yml
- filename: tutorcruncher-recipients-api-openapi.yml
  format: yaml
  label: TutorCruncher Recipients API
  slug: tutorcruncher-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-recipients-api-openapi.yml
- filename: tutorcruncher-reference-api-openapi.yml
  format: yaml
  label: TutorCruncher Reference API
  slug: tutorcruncher-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-reference-api-openapi.yml
- filename: tutorcruncher-services-api-openapi.yml
  format: yaml
  label: TutorCruncher Services API
  slug: tutorcruncher-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-services-api-openapi.yml
- filename: tutorcruncher-webhooks-api-openapi.yml
  format: yaml
  label: TutorCruncher Webhooks API
  slug: tutorcruncher-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tutorcruncher Authentication
name_suffix: Authentication
oauth_flows: []
overview: TutorCruncher secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TutorCruncher
provider_slug: tutorcruncher
scheme_count: 1
schemes:
- description: 'Private API key sent as: Authorization: token <API KEY>'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/tutorcruncher-openapi.yml
  type: apiKey
slug: tutorcruncher-authentication
source_filename: tutorcruncher-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tutorcruncher-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Private API key sent as: Authorization: token <API KEY>'\n  sources:\n  - openapi/tutorcruncher-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/authentication/tutorcruncher-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Tutoring
- Education
- Business Management
- Scheduling
- Invoicing
- Payments
- EdTech
---
