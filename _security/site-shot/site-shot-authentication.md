---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Site-Shot API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Site Shot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Site-Shot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Site-Shot
provider_slug: site-shot
scheme_count: 1
schemes:
- evidence: Site‑Shot agent actions use OAuth 2.0 authorization code flow with scoped access tokens.
  how_to_obtain: Configure a confidential OAuth client with a client secret and use the authorization code flow (no PKCE required).
  name: SiteShotOAuth
  scopes:
  - account:read
  - usage:read
  - billing:checkout
  - api_key:read
  type: oauth2
slug: site-shot-authentication
source_filename: site-shot-authentication.yml
source_heading: Authentication Profile
source_url: https://www.site-shot.com/api/v1/agent/docs/api-key.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.site-shot.com/api/v1/agent/docs/api-key.md\nsources:\n- https://www.site-shot.com/api/v1/agent/docs/api-key.md\n- https://www.site-shot.com/pricing/\n- https://www.site-shot.com/api/v1/agent/docs/auth.md\n- https://www.site-shot.com/start/\ndescription: Authentication methods for Site-Shot API\nschemes:\n- type: oauth2\n  name: SiteShotOAuth\n  evidence: Site‑Shot agent actions use OAuth 2.0 authorization code flow with scoped access tokens.\n  scopes:\n  - account:read\n  - usage:read\n  - billing:checkout\n  - api_key:read\n  how_to_obtain: Configure a confidential OAuth client with a client secret and use the authorization code flow (no PKCE required).\ndocs: https://www.site-shot.com/api/v1/agent/docs/api-key.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/site-shot/authentication/site-shot-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Screenshot
- API
- Automation
- Web
---
