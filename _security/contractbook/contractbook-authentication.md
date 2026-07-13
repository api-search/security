---
api_key_in: []
api_specs:
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Documents API
  slug: contractbook-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Templates API
  slug: contractbook-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Document Sharing API
  slug: contractbook-document-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Automations API
  slug: contractbook-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Spaces API
  slug: contractbook-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Attachments API
  slug: contractbook-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Contractbook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contractbook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Contractbook
provider_slug: contractbook
scheme_count: 1
schemes:
- description: 'Bearer API key created in Contractbook profile settings (shown only once on creation) and passed as ''Authorization: Bearer YOUR_API_KEY''. Separate keys exist for the staging and production environments. API access is a paid add-on available on the Centralize and Accelerate plans.'
  name: authorization
  scheme: bearer
  sources:
  - openapi/contractbook-openapi.json
  - https://api.contractbook.com/v3/docs
  type: http
slug: contractbook-authentication
source_filename: contractbook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contractbook-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  description: 'Bearer API key created in Contractbook profile settings (shown only once on\n    creation) and passed as ''Authorization: Bearer YOUR_API_KEY''. Separate keys exist for\n    the staging and production environments. API access is a paid add-on available on the Centralize\n    and Accelerate plans.'\n  sources:\n  - openapi/contractbook-openapi.json\n  - https://api.contractbook.com/v3/docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/authentication/contractbook-authentication.yml
summary_line: http · 1 scheme
tags:
- Contract Management
- CLM
- Contract Lifecycle
- Legal
- eSignature
- Contracts
- Document Automation
- LegalTech
---
