---
api_key_in: []
api_specs:
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Issuers API
  slug: badgr-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr BadgeClasses API
  slug: badgr-badgeclasses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Assertions (Awarded Badges) API
  slug: badgr-assertions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Backpack API
  slug: badgr-backpack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Collections API
  slug: badgr-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Users API
  slug: badgr-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Authentication API
  slug: badgr-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Badgr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Badgr secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Badgr
provider_slug: badgr
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 3
    tokenUrl: https://api.badgr.io/o/token
  - authorizationUrl: https://api.badgr.io/o/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.badgr.io/o/token
  name: OAuth2
  sources:
  - openapi/badgr-openapi.yml
  type: oauth2
slug: badgr-authentication
source_filename: badgr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/badgr-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.badgr.io/o/token\n    scopes: 3\n  - flow: authorizationCode\n    authorizationUrl: https://api.badgr.io/o/authorize\n    tokenUrl: https://api.badgr.io/o/token\n    scopes: 3\n  sources:\n  - openapi/badgr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/authentication/badgr-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Digital Badges
- Open Badges
- Micro-Credentials
- Credentialing
- Verifiable Credentials
- Education
- Open Source
---
