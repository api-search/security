---
api_key_in: []
api_specs:
- filename: adobe-pdf-services-api-openapi.yml
  format: yaml
  label: Adobe PDF Services API
  slug: adobe-pdf-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-pdf-services-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adobe
provider_slug: adobe
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained via client credentials grant from Adobe Identity Management Service (IMS). Generate credentials in the Adobe Developer Console and exchange them for an access token at https://ims-na1.adobelogin.com/ims/token/v3.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-pdf-services-api-openapi.yml
  type: http
slug: adobe-authentication
source_filename: adobe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-pdf-services-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained via client credentials grant from Adobe Identity\n    Management Service (IMS). Generate credentials in the Adobe Developer Console and exchange\n    them for an access token at https://ims-na1.adobelogin.com/ims/token/v3.\n  sources:\n  - openapi/adobe-pdf-services-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/authentication/adobe-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 1000
- Analytics
- Creative Cloud
- Digital Asset Management
- Document Services
- E-Commerce
- E-Signatures
- Experience Cloud
- Generative AI
- Marketing
- PDF
- Work Management
---
