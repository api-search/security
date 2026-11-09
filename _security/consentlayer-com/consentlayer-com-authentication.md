---
anonymous_access: false
api_key_in: []
api_specs:
- filename: consentlayer-com-openapi-generated.yml
  format: yaml
  label: ConsentLayer API
  slug: consentlayer-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consentlayer-com/openapi/_ae-authored/consentlayer-com-openapi-generated.yml
auth_types: []
description: Authentication methods for ConsentLayer API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Consentlayer Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConsentLayer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ConsentLayer
provider_slug: consentlayer-com
scheme_count: 2
schemes:
- evidence: 'Pass your API key in the Authorization header:'
  header: Authorization
  how_to_obtain: Create keys in the dashboard under Account > API Keys.
  location: header
  name: Authorization
  type: http-bearer
- evidence: The API also supports OAuth 2.0 authorization code flow with PKCE for browser-based applications.
  flows:
  - authorization_code
  how_to_obtain: See the dashboard OAuth settings to register a client.
  name: OAuth 2.0
  type: oauth2
slug: consentlayer-com-authentication
source_filename: consentlayer-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.consentlayer.com/docs/api-reference/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.consentlayer.com/docs/api-reference/authentication\nsources:\n- https://docs.consentlayer.com/docs/api-reference/authentication\n- https://docs.consentlayer.com/docs/quickstart\ndescription: Authentication methods for ConsentLayer API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Pass your API key in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys in the dashboard under Account > API Keys.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The API also supports OAuth 2.0 authorization code flow with PKCE for browser-based applications.\n  flows:\n  - authorization_code\n  how_to_obtain: See the dashboard OAuth settings to register a client.\ndocs: https://docs.consentlayer.com/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/consentlayer-com/authentication/consentlayer-com-authentication.yml
summary_line: 2 schemes
tags:
- Cookie Consent
- AI Integration
- Tracker Blocking
- Privacy Compliance
- Consent Logging
---
