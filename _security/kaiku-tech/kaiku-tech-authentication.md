---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Kaiku APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kaiku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaiku declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kaiku
provider_slug: kaiku-tech
scheme_count: 2
schemes:
- evidence: 'Header What goes in it Authorization: Bearer <token> The token. Preferred.'
  header: Authorization
  how_to_obtain: Create a personal access token in Settings → Connect over MCP tab and use it as the bearer token.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Authorization: Basic … Your email (or username) and the token in place of a password — the form tools written for the cloud edition of the tracker use.'
  header: Authorization
  how_to_obtain: Create a personal access token in Settings → Connect over MCP tab and use the email (or username) as the username and the token as the password in a Basic Authorization header.
  location: header
  name: Basic token
  type: http-basic
slug: kaiku-tech-authentication
source_filename: kaiku-tech-authentication.yml
source_heading: Authentication Profile
source_url: https://kaiku.tech/en/docs/connect
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kaiku.tech/en/docs/connect\nsources:\n- https://kaiku.tech/en/docs/connect\ndescription: Authentication methods for Kaiku APIs\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Header What goes in it Authorization: Bearer <token> The token. Preferred.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal access token in Settings → Connect over MCP tab and use it as the bearer token.\n- type: http-basic\n  name: Basic token\n  evidence: 'Authorization: Basic … Your email (or username) and the token in place of a password — the form tools written for the cloud edition\n    of the tracker use.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal access token in Settings → Connect over MCP tab and use the email (or username) as the username and the token\n    as the password in a Basic Authorization header.\n\
  note: No OAuth2, API key, JWT, HMAC, mTLS, or other schemes are documented on the page.\ndocs: https://kaiku.tech/en/docs/connect\n"
source_yaml_url: https://artifacts.apis.io/kaiku-tech/authentication/kaiku-tech-authentication.yml
summary_line: 2 schemes
tags:
- Task Tracker
- Wiki
- AI Agents
- Collaboration
- Privacy
---
