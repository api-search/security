---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nitrino-ai-openapi-generated.yml
  format: yaml
  label: Nitrino API
  slug: nitrino-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nitrino-ai/openapi/_ae-authored/nitrino-ai-openapi-generated.yml
auth_types: []
description: Authentication methods published on the page
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nitrino Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nitrino declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nitrino
provider_slug: nitrino-ai
scheme_count: 1
schemes:
- authorize_url: GET /oauth/authorize?response_type=code&code_challenge_method=S256&…
  evidence: The program runs OAuth 2.1 with PKCE and gets a token for one workspace — with exactly the scopes it was granted.
  flows:
  - authorization_code
  how_to_obtain: POST /oauth/register
  name: OAuth 2.1 with PKCE
  scopes:
  - inbox:read
  - inbox:write
  - people:read
  - people:write
  - products:read
  - products:write
  - companies:read
  - companies:write
  - deals:read
  - deals:write
  - segments:read
  - segments:write
  - campaigns:read
  - campaigns:write
  - agents:read
  - agents:write
  - channels:read
  - channels:write
  - workspace:read
  - workspace:write
  - calendar:read
  - calendar:write
  - routing:read
  - routing:write
  - contacts:write
  - archive:read
  - archive:write
  - dashboard:read
  - billing:read
  - events:read
  - events:write
  type: oauth2
slug: nitrino-ai-authentication
source_filename: nitrino-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://nitrino.ai/docs/auth
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nitrino.ai/docs/auth\nsources:\n- https://nitrino.ai/docs/auth\ndescription: Authentication methods published on the page\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: The program runs OAuth 2.1 with PKCE and gets a token for one workspace — with exactly the scopes it was granted.\n  flows:\n  - authorization_code\n  authorize_url: GET /oauth/authorize?response_type=code&code_challenge_method=S256&…\n  scopes:\n  - inbox:read\n  - inbox:write\n  - people:read\n  - people:write\n  - products:read\n  - products:write\n  - companies:read\n  - companies:write\n  - deals:read\n  - deals:write\n  - segments:read\n  - segments:write\n  - campaigns:read\n  - campaigns:write\n  - agents:read\n  - agents:write\n  - channels:read\n  - channels:write\n  - workspace:read\n  - workspace:write\n  - calendar:read\n  - calendar:write\n  - routing:read\n  - routing:write\n\
  \  - contacts:write\n  - archive:read\n  - archive:write\n  - dashboard:read\n  - billing:read\n  - events:read\n  - events:write\n  how_to_obtain: POST /oauth/register\ndocs: https://nitrino.ai/docs/auth\n"
source_yaml_url: https://artifacts.apis.io/nitrino-ai/authentication/nitrino-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Sales Automation
- B2B
- Multi-Channel Outreach
- CRM Integration
---
