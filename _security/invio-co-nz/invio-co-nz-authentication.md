---
anonymous_access: false
api_key_in: []
api_specs:
- filename: invio-co-nz-openapi-generated.yml
  format: yaml
  label: Invio API
  slug: invio-co-nz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invio-co-nz/openapi/_ae-authored/invio-co-nz-openapi-generated.yml
auth_types: []
description: Invio uses a generated connector URL as the authentication credential. The URL itself (its last path segment) acts as the secret key that must be provided to the client when adding a custom connector.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Invio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Invio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Invio
provider_slug: invio-co-nz
scheme_count: 1
schemes:
- evidence: Treat the URL like a password - anyone who has it can act as this connection inside Invio's guardrails (reads, and drafts that still need your approval - see below).
  how_to_obtain: Generate the connector URL in Invio's Settings → Connectors → Add custom connector screen; the URL is shown once in an amber box and must be copied directly.
  name: connector URL
  type: other
slug: invio-co-nz-authentication
source_filename: invio-co-nz-authentication.yml
source_heading: Authentication Profile
source_url: https://www.invio.co.nz/guides/xero-mcp-setup
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.invio.co.nz/guides/xero-mcp-setup\nsources:\n- https://www.invio.co.nz/guides/xero-mcp-setup\ndescription: Invio uses a generated connector URL as the authentication credential. The URL itself (its last path segment) acts as the secret\n  key that must be provided to the client when adding a custom connector.\nschemes:\n- type: other\n  name: connector URL\n  evidence: Treat the URL like a password - anyone who has it can act as this connection inside Invio's guardrails (reads, and drafts that still\n    need your approval - see below).\n  how_to_obtain: Generate the connector URL in Invio's Settings → Connectors → Add custom connector screen; the URL is shown once in an amber\n    box and must be copied directly.\ndocs: https://www.invio.co.nz/guides/xero-mcp-setup\n"
source_yaml_url: https://artifacts.apis.io/invio-co-nz/authentication/invio-co-nz-authentication.yml
summary_line: 1 scheme
tags:
- Invoicing
- NZ
- Software-as-a-Service
- Small Business
- Fintech
---
