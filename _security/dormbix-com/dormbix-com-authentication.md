---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dormbix-com-ai-feed-json-api-openapi.yml
  format: yaml
  label: DormBix Ai Feed.json API
  slug: dormbix-com-ai-feed-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dormbix-com/openapi/dormbix-com-ai-feed-json-api-openapi.yml
- filename: dormbix-com-public-api-openapi.yml
  format: yaml
  label: DormBix Public API
  slug: dormbix-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dormbix-com/openapi/dormbix-com-public-api-openapi.yml
auth_types: []
description: DormBix uses OAuth 2.1 with the authorization code flow (PKCE S256) for authentication. The obtained access token is sent in the HTTP Authorization header as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dormbix Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DormBix declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DormBix
provider_slug: dormbix-com
scheme_count: 1
schemes:
- authorize_url: /api/oauth/authorize
  evidence: Auth OAuth 2.1 (authorization code + PKCE S256, public client)
  flows:
  - authorization_code
  how_to_obtain: Public client registers via the dynamic client registration endpoint (/api/oauth/register) and performs the authorization code flow with PKCE to receive a token.
  name: OAuth 2.1
  type: oauth2
slug: dormbix-com-authentication
source_filename: dormbix-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.dormbix.com/developers
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.dormbix.com/developers\nsources:\n- https://www.dormbix.com/developers\ndescription: DormBix uses OAuth 2.1 with the authorization code flow (PKCE S256) for authentication. The obtained access token is sent in the\n  HTTP Authorization header as a Bearer token.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Auth OAuth 2.1 (authorization code + PKCE S256, public client)\n  flows:\n  - authorization_code\n  authorize_url: /api/oauth/authorize\n  how_to_obtain: Public client registers via the dynamic client registration endpoint (/api/oauth/register) and performs the authorization code\n    flow with PKCE to receive a token.\nnote: 'The access token must be sent in the request header: Authorization: Bearer <TOKEN>.'\ndocs: https://www.dormbix.com/developers\n"
source_yaml_url: https://artifacts.apis.io/dormbix-com/authentication/dormbix-com-authentication.yml
summary_line: 1 scheme
tags:
- Dormitory Management
- Artificial Intelligence
- Billing Automation
- Thai Market
- Software-as-a-Service
---
