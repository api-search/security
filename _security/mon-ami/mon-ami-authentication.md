---
api_key_in: []
api_specs:
- filename: mon-ami-openapi.yml
  format: yaml
  label: Mon Ami REST API
  slug: mon-ami-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mon Ami Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mon Ami secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mon Ami
provider_slug: mon-ami
scheme_count: 1
schemes:
- credential: uid:secret
  location: Authorization header
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mon-ami-openapi.yml
  type: http
slug: mon-ami-authentication
source_filename: mon-ami-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.monami.io/\ndocs: https://docs.monami.io/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Mon Ami uses HTTP Basic authentication. Credentials are a uid and secret pair\n  passed in the Authorization header as \"Basic base64(uid:secret)\". API credentials\n  are provisioned by Mon Ami (contact the team via the docs to obtain access).\n  No OAuth 2.0 or API-key-header scheme is documented.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    credential: uid:secret\n    location: Authorization header\n    sources: [openapi/mon-ami-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/authentication/mon-ami-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Aging Services
- Disability Services
- Case Management
- Care Coordination
- HL7 FHIR
- HIPAA
---
