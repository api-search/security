---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leadrecorder-com-openapi-generated.yml
  format: yaml
  label: Lead Recorder API
  slug: leadrecorder-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadrecorder-com/openapi/_ae-authored/leadrecorder-com-openapi-generated.yml
auth_types: []
description: Lead Recorder authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lead Recorder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lead Recorder declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lead Recorder
provider_slug: leadrecorder-com
scheme_count: 1
schemes:
- authorize_url: https://www.leadrecorder.com/oauth/authorize
  evidence: 'https://www.leadrecorder.com/oauth/authorize: the interactive login/consent screen ... https://www.leadrecorder.com/api/oauth/token: token exchange (authorization_code grant, PKCE required)'
  flows:
  - authorization_code
  how_to_obtain: Obtain client credentials via Dynamic Client Registration at https://www.leadrecorder.com/api/oauth/register and complete the interactive login/consent screen.
  name: Lead Recorder OAuth
  type: oauth2
slug: leadrecorder-com-authentication
source_filename: leadrecorder-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.leadrecorder.com/docs
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.leadrecorder.com/docs\nsources:\n- https://www.leadrecorder.com/docs\n- https://www.leadrecorder.com/docs/getting-started\n- https://www.leadrecorder.com/docs/grok-mcp-server\ndescription: Lead Recorder authentication\nschemes:\n- type: oauth2\n  name: Lead Recorder OAuth\n  evidence: 'https://www.leadrecorder.com/oauth/authorize: the interactive login/consent screen ... https://www.leadrecorder.com/api/oauth/token:\n    token exchange (authorization_code grant, PKCE required)'\n  flows:\n  - authorization_code\n  authorize_url: https://www.leadrecorder.com/oauth/authorize\n  how_to_obtain: Obtain client credentials via Dynamic Client Registration at https://www.leadrecorder.com/api/oauth/register and complete the\n    interactive login/consent screen.\ndocs: https://www.leadrecorder.com/docs\n"
source_yaml_url: https://artifacts.apis.io/leadrecorder-com/authentication/leadrecorder-com-authentication.yml
summary_line: 1 scheme
tags:
- Marketing
- Attribution
- Lead Tracking
- Software-as-a-Service
- Analytics
---
