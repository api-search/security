---
anonymous_access: false
api_key_in: []
api_specs:
- filename: loopwise-com-openapi-generated.yml
  format: yaml
  label: Loopwise API
  slug: loopwise-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopwise-com/openapi/_ae-authored/loopwise-com-openapi-generated.yml
auth_types: []
description: Loopwise uses the Authorization Code flow with PKCE (RFC 7636).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Loopwise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loopwise declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Loopwise
provider_slug: loopwise-com
scheme_count: 1
schemes:
- authorize_url: https://your-school-domain.com/oauth/authorize
  evidence: 'Loopwise uses the Authorization Code flow with PKCE (RFC 7636):'
  flows:
  - authorization_code
  how_to_obtain: Register an OAuth application in the school admin UI (Settings > OAuth Applications) to receive a client_id and client_secret, or use the vendor registration endpoint for pre‑registered platforms.
  name: Loopwise OAuth
  scopes:
  - openid
  - profile
  - email
  - courses:read
  - courses:write
  - students:read
  - students:write
  - analytics:read
  - curriculum:read
  - curriculum:write
  - orders:read
  - school:read
  type: oauth2
slug: loopwise-com-authentication
source_filename: loopwise-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.loopwise.com/guides/oauth-quickstart
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.loopwise.com/guides/oauth-quickstart\nsources:\n- https://docs.loopwise.com/guides/oauth-quickstart\n- https://docs.loopwise.com/guides/managing-applications\n- https://docs.loopwise.com/concepts/oauth-overview\n- https://docs.loopwise.com/reference/errors\ndescription: Loopwise uses the Authorization Code flow with PKCE (RFC 7636).\nschemes:\n- type: oauth2\n  name: Loopwise OAuth\n  evidence: 'Loopwise uses the Authorization Code flow with PKCE (RFC 7636):'\n  flows:\n  - authorization_code\n  authorize_url: https://your-school-domain.com/oauth/authorize\n  scopes:\n  - openid\n  - profile\n  - email\n  - courses:read\n  - courses:write\n  - students:read\n  - students:write\n  - analytics:read\n  - curriculum:read\n  - curriculum:write\n  - orders:read\n  - school:read\n  how_to_obtain: Register an OAuth application in the school admin UI (Settings > OAuth Applications)\
  \ to receive a client_id and client_secret,\n    or use the vendor registration endpoint for pre‑registered platforms.\ndocs: https://docs.loopwise.com/guides/oauth-quickstart\n"
source_yaml_url: https://artifacts.apis.io/loopwise-com/authentication/loopwise-com-authentication.yml
summary_line: 1 scheme
tags:
- Education
- Online Courses
- AI Integration
- Membership
- Software-as-a-Service
---
