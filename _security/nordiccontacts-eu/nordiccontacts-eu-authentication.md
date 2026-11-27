---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published by NordicContacts
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NordicContacts Authentication
name_suffix: Authentication
oauth_flows: []
overview: NordicContacts declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NordicContacts
provider_slug: nordiccontacts-eu
scheme_count: 1
schemes:
- evidence: 'Clients without OAuth support must send an "Authorization: Bearer" header with a valid manual MCP access token.'
  header: Authorization
  how_to_obtain: Create a manual MCP access token in the account token management page; the token is shown once at creation.
  location: header
  name: Bearer Token
  type: http-bearer
slug: nordiccontacts-eu-authentication
source_filename: nordiccontacts-eu-authentication.yml
source_heading: Authentication Profile
source_url: https://nordiccontacts.eu/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nordiccontacts.eu/.well-known/oauth-authorization-server\nsources:\n- https://nordiccontacts.eu/.well-known/oauth-authorization-server\n- https://nordiccontacts.eu/en/guides/hubspot\n- https://nordiccontacts.eu/en/agents/docs\ndescription: Authentication methods published by NordicContacts\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'Clients without OAuth support must send an \"Authorization: Bearer\" header with a valid manual MCP access token.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a manual MCP access token in the account token management page; the token is shown once at creation.\ndocs: https://nordiccontacts.eu/.well-known/oauth-authorization-server\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/nordiccontacts-eu/authentication/nordiccontacts-eu-authentication.yml
summary_line: 1 scheme
tags:
- B2B
- Data
- Contacts
- Artificial Intelligence
- MCP
---
