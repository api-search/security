---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bridgetown-builders-core-openapi-generated.yml
  format: yaml
  label: Bridge Town core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgetown-builders/openapi/_ae-authored/bridgetown-builders-core-openapi-generated.yml
- filename: bridgetown-builders-getting-started-openapi-generated.yml
  format: yaml
  label: Bridge Town getting started API
  slug: getting-started-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgetown-builders/openapi/_ae-authored/bridgetown-builders-getting-started-openapi-generated.yml
- filename: bridgetown-builders-guides-openapi-generated.yml
  format: yaml
  label: Bridge Town guides API
  slug: guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgetown-builders/openapi/_ae-authored/bridgetown-builders-guides-openapi-generated.yml
auth_types: []
description: Authentication schemes published for Bridge Town
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bridge Town Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bridge Town declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bridge Town
provider_slug: bridgetown-builders
scheme_count: 1
schemes:
- authorize_url: https://api.bridgetown.builders/authorize
  evidence: '"authorization_endpoint":"https://api.bridgetown.builders/authorize"'
  flows:
  - authorization_code
  how_to_obtain: Sign in to Bridge Town in the browser tab that opens and approve access.
  name: OAuth2
  scopes:
  - openid
  - profile
  - email
  - offline_access
  - models:read
  - models:write
  - runs:execute
  - history:read
  - data:read
  - data:write
  - sheets:read
  - sheets:write
  - sharing:manage
  token_url: https://api.bridgetown.builders/oauth/token
  type: oauth2
slug: bridgetown-builders-authentication
source_filename: bridgetown-builders-authentication.yml
source_heading: Authentication Profile
source_url: https://api.bridgetown.builders/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.bridgetown.builders/.well-known/oauth-protected-resource\nsources:\n- https://api.bridgetown.builders/.well-known/oauth-protected-resource\n- https://api.bridgetown.builders/.well-known/oauth-authorization-server\n- https://www.bridgetown.builders/docs/getting-started/claude-code-plugin\n- https://www.bridgetown.builders/docs/getting-started/overview\ndescription: Authentication schemes published for Bridge Town\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"authorization_endpoint\":\"https://api.bridgetown.builders/authorize\"'\n  flows:\n  - authorization_code\n  token_url: https://api.bridgetown.builders/oauth/token\n  authorize_url: https://api.bridgetown.builders/authorize\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  - models:read\n  - models:write\n  - runs:execute\n  - history:read\n  - data:read\n  - data:write\n  - sheets:read\n\
  \  - sheets:write\n  - sharing:manage\n  how_to_obtain: Sign in to Bridge Town in the browser tab that opens and approve access.\ndocs: https://api.bridgetown.builders/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/bridgetown-builders/authentication/bridgetown-builders-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Artificial Intelligence
- FP&A
- Collaboration
- Version Control
- Company
---
