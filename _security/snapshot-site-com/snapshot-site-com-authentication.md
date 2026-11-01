---
anonymous_access: false
api_key_in: []
api_specs:
- filename: snapshot-site-com-openapi-generated.yml
  format: yaml
  label: snapshot-site-com API
  slug: snapshot-site-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapshot-site-com/openapi/_ae-authored/snapshot-site-com-openapi-generated.yml
auth_types: []
description: Authentication uses an API key sent in a custom header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Snapshot Site Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: snapshot-site-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: snapshot-site-com
provider_slug: snapshot-site-com
scheme_count: 1
schemes:
- evidence: Send the account API key through the x‑snapshotsiteapi‑key header on HTTPS requests to the documented endpoint.
  header: x-snapshotsiteapi-key
  how_to_obtain: Provision the key into a trusted runtime through secret management.
  location: header
  name: Snapshot Site API Key
  type: apiKey
slug: snapshot-site-com-authentication
source_filename: snapshot-site-com-authentication.yml
source_heading: Authentication Profile
source_url: https://snapshot-site.com/screenshot-api-authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://snapshot-site.com/screenshot-api-authentication\nsources:\n- https://snapshot-site.com/screenshot-api-authentication\n- https://snapshot-site.com/posts/a-recipe-for-clean-onboarding-tour-screenshots\n- https://snapshot-site.com/posts/use-snapshot-site-mcp-with-claude-desktop-and-cursor\ndescription: Authentication uses an API key sent in a custom header.\nschemes:\n- type: apiKey\n  name: Snapshot Site API Key\n  evidence: Send the account API key through the x‑snapshotsiteapi‑key header on HTTPS requests to the documented endpoint.\n  location: header\n  header: x-snapshotsiteapi-key\n  how_to_obtain: Provision the key into a trusted runtime through secret management.\ndocs: https://snapshot-site.com/screenshot-api-authentication\n"
source_yaml_url: https://artifacts.apis.io/snapshot-site-com/authentication/snapshot-site-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Screenshot
- API
- AI
- Monitoring
---
