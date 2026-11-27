---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adbtd-com-openapi-generated.yml
  format: yaml
  label: adbtd API
  slug: adbtd-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adbtd-com/openapi/_ae-authored/adbtd-com-openapi-generated.yml
auth_types: []
description: Authentication for adbtd MCP uses OAuth 2.1 with dynamic client registration and PKCE. The client is sent to a browser to approve and an API key is auto‑minted.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: adbtd Authentication
name_suffix: Authentication
oauth_flows: []
overview: adbtd declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: adbtd
provider_slug: adbtd-com
scheme_count: 1
schemes:
- authorize_url: https://adbtd.com/oauth/authorize
  evidence: OAuth-based authorization, revocable from your dashboard at any time.
  flows:
  - authorization_code
  how_to_obtain: On first connection the browser opens to the authorize URL where the user approves the request; an API key is auto‑minted under the user's account.
  name: OAuth 2.1
  type: oauth2
slug: adbtd-com-authentication
source_filename: adbtd-com-authentication.yml
source_heading: Authentication Profile
source_url: https://adbtd.com/blog/cold-email-infrastructure-setup-2026
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://adbtd.com/blog/cold-email-infrastructure-setup-2026\nsources:\n- https://adbtd.com/blog/cold-email-infrastructure-setup-2026\n- https://adbtd.com/mcp\ndescription: Authentication for adbtd MCP uses OAuth 2.1 with dynamic client registration and PKCE. The client is sent to a browser to approve\n  and an API key is auto‑minted.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: OAuth-based authorization, revocable from your dashboard at any time.\n  flows:\n  - authorization_code\n  authorize_url: https://adbtd.com/oauth/authorize\n  how_to_obtain: On first connection the browser opens to the authorize URL where the user approves the request; an API key is auto‑minted under\n    the user's account.\ndocs: https://adbtd.com/blog/cold-email-infrastructure-setup-2026\n"
source_yaml_url: https://artifacts.apis.io/adbtd-com/authentication/adbtd-com-authentication.yml
summary_line: 1 scheme
tags:
- Email Infrastructure
- SMTP
- IMAP
- Dedicated IP
- Deliverability
- Webhook
- MCP
---
