---
anonymous_access: false
api_key_in: []
api_specs:
- filename: echoapi-openapi-generated.yml
  format: yaml
  label: EchoAPI API
  slug: echoapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echoapi/refs/heads/main/openapi/_ae-authored/echoapi-openapi-generated.yml
auth_types: []
description: Authentication methods as published on the page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Echoapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: EchoAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EchoAPI
provider_slug: echoapi
scheme_count: 1
schemes:
- authorize_url: https://github.com/login/oauth/authorize
  evidence: EchoAPI supports OAuth 2.0 authentication starting from version 2.0.13.
  flows:
  - authorization_code
  how_to_obtain: Create a GitHub OAuth Application, obtain the Client ID and Client Secret, then use EchoAPI's Get Token button to retrieve an access token.
  name: OAuth 2.0
  type: oauth2
slug: echoapi-authentication
source_filename: echoapi-authentication.yml
source_heading: Authentication Profile
source_url: https://www.echoapi.com/wiki/docs/oauth2
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.echoapi.com/wiki/docs/oauth2\nsources:\n- https://www.echoapi.com/wiki/docs/oauth2\ndescription: Authentication methods as published on the page.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: EchoAPI supports OAuth 2.0 authentication starting from version 2.0.13.\n  flows:\n  - authorization_code\n  authorize_url: https://github.com/login/oauth/authorize\n  how_to_obtain: Create a GitHub OAuth Application, obtain the Client ID and Client Secret, then use EchoAPI's Get Token button to retrieve an\n    access token.\ndocs: https://www.echoapi.com/wiki/docs/oauth2\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echoapi/refs/heads/main/authentication/echoapi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API Platform
- Integration
- Developer Tools
- AI-powered
- Documentation
---
