---
api_key_in:
- header
api_specs:
- filename: boldsign-branding-api-openapi.yml
  format: yaml
  label: BoldSign Branding API
  slug: boldsign-branding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-branding-api-openapi.yml
- filename: boldsign-contacts-api-openapi.yml
  format: yaml
  label: BoldSign Contacts API
  slug: boldsign-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-contacts-api-openapi.yml
- filename: boldsign-custom-field-api-openapi.yml
  format: yaml
  label: BoldSign Custom Field API
  slug: boldsign-custom-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-custom-field-api-openapi.yml
- filename: boldsign-document-api-openapi.yml
  format: yaml
  label: BoldSign Document API
  slug: boldsign-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-document-api-openapi.yml
- filename: boldsign-groupcontacts-api-openapi.yml
  format: yaml
  label: BoldSign GroupContacts API
  slug: boldsign-groupcontacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-groupcontacts-api-openapi.yml
- filename: boldsign-identity-verification-api-openapi.yml
  format: yaml
  label: BoldSign Identity Verification API
  slug: boldsign-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-identity-verification-api-openapi.yml
- filename: boldsign-plan-api-openapi.yml
  format: yaml
  label: BoldSign Plan API
  slug: boldsign-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-plan-api-openapi.yml
- filename: boldsign-sender-identities-api-openapi.yml
  format: yaml
  label: BoldSign Sender Identities API
  slug: boldsign-sender-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-sender-identities-api-openapi.yml
- filename: boldsign-teams-api-openapi.yml
  format: yaml
  label: BoldSign Teams API
  slug: boldsign-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-teams-api-openapi.yml
- filename: boldsign-template-api-openapi.yml
  format: yaml
  label: BoldSign Template API
  slug: boldsign-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-template-api-openapi.yml
- filename: boldsign-user-api-openapi.yml
  format: yaml
  label: BoldSign User API
  slug: boldsign-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/openapi/boldsign-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Boldsign Authentication
name_suffix: Authentication
oauth_flows: []
overview: BoldSign secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BoldSign
provider_slug: boldsign
scheme_count: 2
schemes:
- description: 'Format ''Bearer'' [space] [TOKEN]. Ex: ''Bearer [example key]'''
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/boldsign-esignature-openapi.yml
  type: apiKey
- description: 'Format [API-KEY]. Ex: ''abcdef12345'''
  in: header
  name: X-API-KEY
  parameter: X-API-KEY
  sources:
  - openapi/boldsign-esignature-openapi.yml
  type: apiKey
slug: boldsign-authentication
source_filename: boldsign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/boldsign-esignature-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Format ''Bearer'' [space] [TOKEN]. Ex: ''Bearer [example key]'''\n  sources:\n  - openapi/boldsign-esignature-openapi.yml\n- name: X-API-KEY\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: 'Format [API-KEY]. Ex: ''abcdef12345'''\n  sources:\n  - openapi/boldsign-esignature-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/authentication/boldsign-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- E-Signature
- Electronic Signature
- Document-Management
- Embedded Signing
- Webhook
- Templates
- Identity Verification
- Compliance
---
