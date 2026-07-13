---
api_key_in:
- header
api_specs:
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Connection API
  slug: revert-dev-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Unified CRM Contacts API
  slug: revert-dev-crm-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Unified CRM Leads API
  slug: revert-dev-crm-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Unified CRM Deals API
  slug: revert-dev-crm-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Unified CRM Companies API
  slug: revert-dev-crm-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Unified CRM Notes API
  slug: revert-dev-crm-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Unified CRM Tasks API
  slug: revert-dev-crm-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Unified CRM Events API
  slug: revert-dev-crm-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Unified CRM Users API
  slug: revert-dev-crm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert CRM Proxy (Passthrough) API
  slug: revert-dev-crm-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert CRM Properties & Field Mapping API
  slug: revert-dev-crm-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Metadata API
  slug: revert-dev-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
- filename: revert-dev-openapi.yml
  format: yaml
  label: Revert Webhooks API
  slug: revert-dev-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/openapi/revert-dev-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Revert Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revert secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Revert
provider_slug: revert-dev
scheme_count: 1
schemes:
- description: Your Revert API key (private token used from your backend).
  in: header
  name: revertApiToken
  parameter: x-revert-api-token
  sources:
  - openapi/revert-dev-openapi.yml
  type: apiKey
slug: revert-dev-authentication
source_filename: revert-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revert-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: revertApiToken\n  type: apiKey\n  in: header\n  parameter: x-revert-api-token\n  description: Your Revert API key (private token used from your backend).\n  sources:\n  - openapi/revert-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revert-dev/refs/heads/main/authentication/revert-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Unified API
- Integrations
- CRM
- iPaaS
- Open Source
- OAuth
---
