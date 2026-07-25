---
api_key_in: []
api_specs:
- filename: mosey-accounts-api-openapi.yml
  format: yaml
  label: Mosey Accounts API
  slug: mosey-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-accounts-api-openapi.yml
- filename: mosey-agency-accounts-api-openapi.yml
  format: yaml
  label: Mosey Agency Accounts API
  slug: mosey-agency-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-agency-accounts-api-openapi.yml
- filename: mosey-auth-api-openapi.yml
  format: yaml
  label: Mosey Auth API
  slug: mosey-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-auth-api-openapi.yml
- filename: mosey-documents-api-openapi.yml
  format: yaml
  label: Mosey Documents API
  slug: mosey-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-documents-api-openapi.yml
- filename: mosey-handbook-api-openapi.yml
  format: yaml
  label: Mosey Handbook API
  slug: mosey-handbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-handbook-api-openapi.yml
- filename: mosey-legal-entity-api-openapi.yml
  format: yaml
  label: Mosey Legal Entity API
  slug: mosey-legal-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-legal-entity-api-openapi.yml
- filename: mosey-locations-api-openapi.yml
  format: yaml
  label: Mosey Locations API
  slug: mosey-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-locations-api-openapi.yml
- filename: mosey-logins-api-openapi.yml
  format: yaml
  label: Mosey Logins API
  slug: mosey-logins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-logins-api-openapi.yml
- filename: mosey-mail-api-openapi.yml
  format: yaml
  label: Mosey Mail API
  slug: mosey-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-mail-api-openapi.yml
- filename: mosey-regions-api-openapi.yml
  format: yaml
  label: Mosey Regions API
  slug: mosey-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-regions-api-openapi.yml
- filename: mosey-signup-api-openapi.yml
  format: yaml
  label: Mosey Signup API
  slug: mosey-signup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-signup-api-openapi.yml
- filename: mosey-tasks-api-openapi.yml
  format: yaml
  label: Mosey Tasks API
  slug: mosey-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-tasks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mosey Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Mosey secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Mosey
provider_slug: mosey
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: /api/token
  name: OAuth2PasswordBearer
  sources:
  - openapi/mosey-openapi.json
  - openapi/mosey-openapi_v1.json
  - openapi/mosey-openapi_v2.json
  type: oauth2
slug: mosey-authentication
source_filename: mosey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mosey-openapi.json, openapi/mosey-openapi_v1.json, openapi/mosey-openapi_v2.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /api/token\n    scopes: 0\n  sources:\n  - openapi/mosey-openapi.json\n  - openapi/mosey-openapi_v1.json\n  - openapi/mosey-openapi_v2.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/authentication/mosey-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Compliance
- Regulatory Technology
- State Compliance
- Tax
- Payroll
- HR
- Business Operations
---
