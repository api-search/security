---
api_key_in: []
api_specs:
- filename: docs.pdffiller.com
  format: yaml
  label: PDFfiller REST API
  slug: pdffiller-api
  spec_type: OpenAPI
  url: https://docs.pdffiller.com
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pdffiller Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: PDFfiller secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: PDFfiller
provider_slug: pdffiller
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 2
    tokenUrl: https://api.pdffiller.com/v2/oauth/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.pdffiller.com/v2/oauth/token
  name: oauth2
  sources:
  - openapi/pdffiller-pdffiller-api-openapi.yml
  type: oauth2
slug: pdffiller-authentication
source_filename: pdffiller-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pdffiller-pdffiller-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.pdffiller.com/v2/oauth/token\n    scopes: 2\n  - flow: clientCredentials\n    tokenUrl: https://api.pdffiller.com/v2/oauth/token\n    scopes: 2\n  sources:\n  - openapi/pdffiller-pdffiller-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/authentication/pdffiller-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- PDF
- E-Signature
- Document Management
- Form Builder
- PDF Editing
- Electronic Signature
- Document Workflow
---
