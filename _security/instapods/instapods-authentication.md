---
anonymous_access: false
api_key_in: []
api_specs:
- filename: instapods-openapi-generated.yml
  format: yaml
  label: ExpressTech Systems API
  slug: instapods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapods/refs/heads/main/openapi/_ae-authored/instapods-openapi-generated.yml
auth_types: []
description: Authentication methods for InstaPods CLI and API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Instapods Authentication
name_suffix: Authentication
oauth_flows: []
overview: ExpressTech Systems declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ExpressTech Systems
provider_slug: instapods
scheme_count: 1
schemes:
- evidence: instapods login --email you@example.com --use-password
  how_to_obtain: Run `instapods login --email <email> --use-password` and enter your password when prompted; the CLI saves a session token locally.
  name: Email/Password
  type: other
slug: instapods-authentication
source_filename: instapods-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.instapods.com/cli/authentication.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.instapods.com/cli/authentication.md\nsources:\n- https://docs.instapods.com/cli/authentication.md\n- https://docs.instapods.com/mcp/authentication.md\n- https://docs.instapods.com/api-reference/api-tokens.md\n- https://docs.instapods.com/quickstart.md\ndescription: Authentication methods for InstaPods CLI and API\nschemes:\n- type: other\n  name: Email/Password\n  evidence: instapods login --email you@example.com --use-password\n  how_to_obtain: Run `instapods login --email <email> --use-password` and enter your password when prompted; the CLI saves a session token locally.\ndocs: https://docs.instapods.com/cli/authentication.md\nnote: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instapods/refs/heads/main/authentication/instapods-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Deployment
- Cloud
- AI-Integration
- DeveloperTools
---
