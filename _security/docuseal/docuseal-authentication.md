---
api_key_in:
- header
api_specs:
- filename: docuseal-submissions-api-openapi.yml
  format: yaml
  label: DocuSeal Submissions API
  slug: docuseal-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docuseal/refs/heads/main/openapi/docuseal-submissions-api-openapi.yml
- filename: docuseal-submitters-api-openapi.yml
  format: yaml
  label: DocuSeal Submitters API
  slug: docuseal-submitters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docuseal/refs/heads/main/openapi/docuseal-submitters-api-openapi.yml
- filename: docuseal-templates-api-openapi.yml
  format: yaml
  label: DocuSeal Templates API
  slug: docuseal-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docuseal/refs/heads/main/openapi/docuseal-templates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Docuseal Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocuSeal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DocuSeal
provider_slug: docuseal
scheme_count: 1
schemes:
- in: header
  name: AuthToken
  parameter: X-Auth-Token
  sources:
  - openapi/docuseal-docuseal-api-openapi.yml
  type: apiKey
slug: docuseal-authentication
source_filename: docuseal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docuseal-docuseal-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/docuseal-docuseal-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docuseal/refs/heads/main/authentication/docuseal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Signing
- E-Signature
- Electronic Signature
- Document-Management
- PDF
- Templates
- Open-Source
- Webhook
- Embedding
---
