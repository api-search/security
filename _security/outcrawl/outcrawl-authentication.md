---
anonymous_access: false
api_key_in: []
api_specs:
- filename: outcrawl-scrape-api-openapi.yml
  format: yaml
  label: Outcrawl Scrape API
  slug: outcrawl-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcrawl/openapi/outcrawl-scrape-api-openapi.yml
auth_types: []
description: 'Outcrawl supports two bearer authentication schemes: an API key and an OAuth access token. Both are sent in the Authorization header as a Bearer token.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Outcrawl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Outcrawl declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Outcrawl
provider_slug: outcrawl
scheme_count: 1
schemes:
- evidence: An API key is a long-lived credential for your own applications and scripts.
  header: Authorization
  how_to_obtain: Generate and revoke keys from https://outcrawl.ai/console/keys
  location: header
  name: API key
  type: http-bearer
slug: outcrawl-authentication
source_filename: outcrawl-authentication.yml
source_heading: Authentication Profile
source_url: https://outcrawl.ai/docs/api-reference/sessions/choose-who-may-watch-a-session-besides-your-own-api-keys:-`private`-your-organization-the-default-`link`-anyone-
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://outcrawl.ai/docs/api-reference/sessions/choose-who-may-watch-a-session-besides-your-own-api-keys:-`private`-your-organization-the-default-`link`-anyone-\nsources:\n- https://outcrawl.ai/docs/api-reference/sessions/choose-who-may-watch-a-session-besides-your-own-api-keys:-`private`-your-organization-the-default-`link`-anyone-\n- https://outcrawl.ai/docs/api/authentication\n- https://outcrawl.ai/docs/account/authentication\n- https://outcrawl.ai/docs/account/api-keys\ndescription: 'Outcrawl supports two bearer authentication schemes: an API key and an OAuth access token. Both are sent in the Authorization header\n  as a Bearer token.'\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: An API key is a long-lived credential for your own applications and scripts.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate and revoke keys from https://outcrawl.ai/console/keys\n\
  note: No OAuth flow URLs or scopes are documented on the provided pages. 1 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://outcrawl.ai/docs/api-reference/sessions/choose-who-may-watch-a-session-besides-your-own-api-keys:-`private`-your-organization-the-default-`link`-anyone-\n"
source_yaml_url: https://artifacts.apis.io/outcrawl/authentication/outcrawl-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Web Infrastructure
- Data Extraction
- Automation
---
