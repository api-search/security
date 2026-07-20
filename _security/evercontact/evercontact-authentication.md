---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Evercontact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evercontact secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Evercontact
provider_slug: evercontact
scheme_count: 1
schemes:
- bearer_format: ec_live_ / ec_test_ prefixed token
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://www.evercontact.com/api.html
  type: http
slug: evercontact-authentication
source_filename: evercontact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.evercontact.com/api.html\ndocs: https://www.evercontact.com/api.html\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The REST API authenticates with a bearer token in the Authorization header.\n    Live tokens carry an ec_live_ prefix (a sandbox/test mode is offered). Separately,\n    end-user data access to Google Workspace and Microsoft 365 mailboxes is granted\n    via OAuth consent (validated under Google CASA Tier 2), with instant revocation\n    of the OAuth grant by the user.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: ec_live_ / ec_test_ prefixed token\n  in: header\n  header: Authorization\n  sources:\n  - https://www.evercontact.com/api.html\nmailbox_authorization:\n  method: oauth2\n  providers:\n  - Google Workspace\n  - Microsoft 365\n  assurance: Google CASA Tier 2\n  revocation: user-initiated, instant\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evercontact/refs/heads/main/authentication/evercontact-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Contact Management
- Contact Data
- Data Enrichment
- Email
- Signature Parsing
- Data Extraction
- CRM
---
