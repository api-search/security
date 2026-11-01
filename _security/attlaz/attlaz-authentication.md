---
anonymous_access: false
api_key_in: []
api_specs:
- filename: attlaz-openapi-generated.yml
  format: yaml
  label: Attlaz API
  slug: attlaz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attlaz/openapi/_ae-authored/attlaz-openapi-generated.yml
auth_types: []
description: 'The Attlaz API uses OAuth 2.0. Every request to a protected endpoint must include a Bearer access token: Authorization: Bearer <access_token>'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Attlaz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Attlaz declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Attlaz
provider_slug: attlaz
scheme_count: 2
schemes:
- evidence: 'The Attlaz API uses OAuth 2.0 . Every request to a protected endpoint must include a Bearer access token:'
  flows:
  - client_credentials
  - refresh_token
  how_to_obtain: Create an OAuth client to get a client_id and client_secret, then exchange them for an access token at the token endpoint.
  name: OAuth 2.0
  token_url: https://api.attlaz.com/oauth/token
  type: oauth2
- evidence: 'Send the token exactly like any other access token: curl https://api.attlaz.com/1.13/ .. . \ -H "Authorization: Bearer <personal_access_token>"'
  header: Authorization
  how_to_obtain: Create a personal access token (PAT) in the dashboard or via the API; the token secret is shown once at creation.
  location: header
  name: Personal Access Token
  type: http-bearer
slug: attlaz-authentication
source_filename: attlaz-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.attlaz.com/reference/api/auth/
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.attlaz.com/reference/api/auth/\nsources:\n- https://docs.attlaz.com/reference/api/auth/\ndescription: 'The Attlaz API uses OAuth 2.0. Every request to a protected endpoint must include a Bearer access token: Authorization: Bearer <access_token>'\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'The Attlaz API uses OAuth 2.0 . Every request to a protected endpoint must include a Bearer access token:'\n  flows:\n  - client_credentials\n  - refresh_token\n  token_url: https://api.attlaz.com/oauth/token\n  how_to_obtain: Create an OAuth client to get a client_id and client_secret, then exchange them for an access token at the token endpoint.\n- type: http-bearer\n  name: Personal Access Token\n  evidence: 'Send the token exactly like any other access token: curl https://api.attlaz.com/1.13/ .. . \\ -H \"Authorization: Bearer <personal_access_token>\"'\n  location:\
  \ header\n  header: Authorization\n  how_to_obtain: Create a personal access token (PAT) in the dashboard or via the API; the token secret is shown once at creation.\ndocs: https://docs.attlaz.com/reference/api/auth/\n"
source_yaml_url: https://artifacts.apis.io/attlaz/authentication/attlaz-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Integration
- Automation
- Data Visualization
- Workflows
---
