---
api_key_in: []
api_specs:
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Studios API
  slug: shootproof-studios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Events & Galleries API
  slug: shootproof-events-galleries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Photos API
  slug: shootproof-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Clients API
  slug: shootproof-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Orders API
  slug: shootproof-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Contracts API
  slug: shootproof-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Shootproof Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ShootProof secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ShootProof
provider_slug: shootproof
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://auth.shootproof.com/oauth2/authorization/new
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://auth.shootproof.com/oauth2/authorization/token
  name: shootProofAuth
  sources:
  - openapi/shootproof-openapi.yml
  type: oauth2
slug: shootproof-authentication
source_filename: shootproof-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shootproof-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: shootProofAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.shootproof.com/oauth2/authorization/new\n    tokenUrl: https://auth.shootproof.com/oauth2/authorization/token\n    scopes: 5\n  sources:\n  - openapi/shootproof-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/authentication/shootproof-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Photography
- Client Galleries
- Proofing
- Digital Downloads
- Photo Studio Management
- E-Commerce
- SaaS
---
