---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leadfeeder-openapi-generated.yml
  format: yaml
  label: Leadfeeder API
  slug: leadfeeder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfeeder/openapi/_ae-authored/leadfeeder-openapi-generated.yml
auth_types: []
description: 'Leadfeeder API supports two authentication methods: API key and OAuth 2.0.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Leadfeeder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leadfeeder declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Leadfeeder
provider_slug: leadfeeder
scheme_count: 2
schemes:
- evidence: A valid API key must be included in every request using the X-Api-Key header.
  header: X-Api-Key
  how_to_obtain: Generate an API key in the Leadfeeder platform under Settings → Personal → API Keys.
  location: header
  name: X-Api-Key
  type: apiKey
- authorize_url: https://api.leadfeeder.com/v1/oauth/authorize
  evidence: OAuth lets an application call the API on behalf of a Leadfeeder user, with access limited to the scopes that user approved.
  flows:
  - authorization_code
  how_to_obtain: Register an application in Settings > Company > Developer Access > Applications to obtain a Client ID and Client Secret, then follow the Authorization Code with PKCE flow.
  name: Leadfeeder OAuth
  type: oauth2
slug: leadfeeder-authentication
source_filename: leadfeeder-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.leadfeeder.com/api/public/authentication-354547m0
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.leadfeeder.com/api/public/authentication-354547m0\nsources:\n- https://docs.leadfeeder.com/api/public/authentication-354547m0\n- https://docs.leadfeeder.com/api/public/-authentication-and-permissions-370535m0\n- https://help.leadfeeder.com/en/articles/13922448-authentication-methods\n- https://help.leadfeeder.com/en/articles/14534032-api-key-and-permissions\ndescription: 'Leadfeeder API supports two authentication methods: API key and OAuth 2.0.'\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: A valid API key must be included in every request using the X-Api-Key header.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Generate an API key in the Leadfeeder platform under Settings → Personal → API Keys.\n- type: oauth2\n  name: Leadfeeder OAuth\n  evidence: OAuth lets an application call the API on behalf of a Leadfeeder user, with access limited to\
  \ the scopes that user approved.\n  flows:\n  - authorization_code\n  authorize_url: https://api.leadfeeder.com/v1/oauth/authorize\n  how_to_obtain: Register an application in Settings > Company > Developer Access > Applications to obtain a Client ID and Client Secret, then\n    follow the Authorization Code with PKCE flow.\ndocs: https://docs.leadfeeder.com/api/public/authentication-354547m0\n"
source_yaml_url: https://artifacts.apis.io/leadfeeder/authentication/leadfeeder-authentication.yml
summary_line: 2 schemes
tags:
- Company
- B2B
- Analytics
- Lead Generation
- Marketing
---
