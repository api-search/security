---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mostlypdf Authentication
name_suffix: Authentication
oauth_flows: []
overview: MostlyPDF declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MostlyPDF
provider_slug: mostlypdf
scheme_count: 2
schemes:
- description: Bearer token with key starting with sk_
  header: Authorization
  scheme: bearer
  type: http
- description: Alternative header x-api-key accepted
  header: x-api-key
  scheme: bearer
  type: http
slug: mostlypdf-authentication
source_filename: mostlypdf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: searched\nsource: https://mostlypdf.com/docs#auth\nschemes:\n  - type: http\n    scheme: bearer\n    description: Bearer token with key starting with sk_\n    header: Authorization\n  - type: http\n    scheme: bearer\n    description: Alternative header x-api-key accepted\n    header: x-api-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mostlypdf/refs/heads/main/authentication/mostlypdf-authentication.yml
summary_line: 2 schemes
tags:
- Company
- PDF
- API
- Automation
- FreeTools
---
