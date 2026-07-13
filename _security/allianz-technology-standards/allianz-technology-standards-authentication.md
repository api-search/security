---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Allianz Technology Standards Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Allianz Technology Standards secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
scheme_count: 1
schemes:
- description: OAuth2 client credentials for Allianz standards API
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://standards.allianz.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/allianz-technology-standards-compliance.yaml
  type: oauth2
slug: allianz-technology-standards-authentication
source_filename: allianz-technology-standards-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-technology-standards-compliance.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://standards.allianz.com/oauth2/token\n    scopes: 2\n  description: OAuth2 client credentials for Allianz standards API\n  sources:\n  - openapi/allianz-technology-standards-compliance.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/authentication/allianz-technology-standards-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
---
