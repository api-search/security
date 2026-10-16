---
anonymous_access: false
api_key_in: []
api_specs:
- filename: digital-realty-openapi-generated.yml
  format: yaml
  label: Digital Realty API
  slug: digital-realty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-realty/refs/heads/main/openapi/_ae-authored/digital-realty-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Digital Realty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digital Realty declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Digital Realty
provider_slug: digital-realty
scheme_count: 1
schemes:
- evidence: First of all, hit the Access Token request to get the bearer token, which can be used to make calls to any API endpoint.
  flows:
  - client_credentials
  how_to_obtain: Create an App in the Digital Realty portal and use the Client Id and Client Secret from the App as the client_id and client_secret.
  name: OAuth2 Client Credentials
  scopes:
  - playground_api
  token_url: https://playground.digitalrealty.com/v2/auth/token
  type: oauth2
slug: digital-realty-authentication
source_filename: digital-realty-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.digitalrealty.com/docs/getting-started
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.digitalrealty.com/docs/getting-started\nsources:\n- https://developer.digitalrealty.com/docs/getting-started\ndescription: Authentication\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: First of all, hit the Access Token request to get the bearer token, which can be used to make calls to any API endpoint.\n  flows:\n  - client_credentials\n  token_url: https://playground.digitalrealty.com/v2/auth/token\n  scopes:\n  - playground_api\n  how_to_obtain: Create an App in the Digital Realty portal and use the Client Id and Client Secret from the App as the client_id and client_secret.\ndocs: https://developer.digitalrealty.com/docs/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-realty/refs/heads/main/authentication/digital-realty-authentication.yml
summary_line: 1 scheme
tags:
- DataCenter
- Colocation
- Cloud
- Infrastructure
- Sustainability
---
