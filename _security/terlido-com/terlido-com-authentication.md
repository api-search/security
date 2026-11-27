---
anonymous_access: false
api_key_in: []
api_specs:
- filename: terlido-com-openapi-generated.yml
  format: yaml
  label: Terlido API
  slug: terlido-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terlido-com/openapi/_ae-authored/terlido-com-openapi-generated.yml
auth_types: []
description: Authentication methods as published on Terlido pages
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Terlido Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terlido declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Terlido
provider_slug: terlido-com
scheme_count: 1
schemes:
- evidence: Sign-in is OAuth 2.1 with dynamic client registration. An unauthenticated call answers 401 and points at https://terlido.com/.well-known/oauth-protected-resource, which starts the handshake.
  how_to_obtain: dynamic client registration via OAuth 2.1 handshake
  name: MCP OAuth 2.1
  type: oauth2
slug: terlido-com-authentication
source_filename: terlido-com-authentication.yml
source_heading: Authentication Profile
source_url: https://terlido.com/glossary/dmarc
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://terlido.com/glossary/dmarc\nsources:\n- https://terlido.com/glossary/dmarc\n- https://terlido.com/agent_onboarding.md\n- https://help.terlido.com/docs/getting-started/sign-in/\ndescription: Authentication methods as published on Terlido pages\nschemes:\n- type: oauth2\n  name: MCP OAuth 2.1\n  evidence: Sign-in is OAuth 2.1 with dynamic client registration. An unauthenticated call answers 401 and points at https://terlido.com/.well-known/oauth-protected-resource,\n    which starts the handshake.\n  how_to_obtain: dynamic client registration via OAuth 2.1 handshake\ndocs: https://terlido.com/glossary/dmarc\n"
source_yaml_url: https://artifacts.apis.io/terlido-com/authentication/terlido-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email
- Newsletter
- Cold-Email
- AI
---
