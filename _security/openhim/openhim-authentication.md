---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openhim-openapi-generated.yml
  format: yaml
  label: OpenHIM API
  slug: openhim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openhim/openapi/_ae-authored/openhim-openapi-generated.yml
auth_types: []
description: Authentication mechanisms for OpenHIM as documented
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: OpenHIM Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenHIM declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: OpenHIM
provider_slug: openhim
scheme_count: 3
schemes:
- evidence: The encoded token generated would then be used in the Authorization request header for requests to the OpenHIM Core
  header: Authorization
  how_to_obtain: Create a JWT token with the client_id in the sub field and sign it using the configured secret/key
  location: header
  name: JWT
  type: http-bearer
- evidence: 'To be authenticated using the local protocol, you can hit this route: POST https://<server>:8080/authenticate/local'
  how_to_obtain: POST username and password in JSON body to /authenticate/local
  location: body
  name: Local authentication (API)
  type: other
- evidence: 'To be authenticated using OpenID, you can hit this route: POST https://<server>:8080/authenticate/openid'
  how_to_obtain: Obtain an authorization code from the OpenID provider and POST it to /authenticate/openid
  location: body
  name: OpenID authentication (API)
  scopes:
  - openid
  - email
  - profile
  - offline_access
  - roles
  type: other
slug: openhim-authentication
source_filename: openhim-authentication.yml
source_heading: Authentication Profile
source_url: https://openhim.org/docs/configuration/authentication/
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://openhim.org/docs/configuration/authentication/\nsources:\n- https://openhim.org/docs/configuration/authentication/\n- https://openhim.org/docs/api/introduction/authentication/\n- https://openhim.org/docs/getting-started/prerequisites/\n- https://openhim.org/docs/getting-started/install/\ndescription: Authentication mechanisms for OpenHIM as documented\nschemes:\n- type: http-bearer\n  name: JWT\n  evidence: The encoded token generated would then be used in the Authorization request header for requests to the OpenHIM Core\n  location: header\n  header: Authorization\n  how_to_obtain: Create a JWT token with the client_id in the sub field and sign it using the configured secret/key\n- type: other\n  name: Local authentication (API)\n  evidence: 'To be authenticated using the local protocol, you can hit this route: POST https://<server>:8080/authenticate/local'\n  location:\
  \ body\n  how_to_obtain: POST username and password in JSON body to /authenticate/local\n- type: other\n  name: OpenID authentication (API)\n  evidence: 'To be authenticated using OpenID, you can hit this route: POST https://<server>:8080/authenticate/openid'\n  location: body\n  scopes:\n  - openid\n  - email\n  - profile\n  - offline_access\n  - roles\n  how_to_obtain: Obtain an authorization code from the OpenID provider and POST it to /authenticate/openid\ndocs: https://openhim.org/docs/configuration/authentication/\nnote: 5 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/openhim/authentication/openhim-authentication.yml
summary_line: 3 schemes
tags:
- Health
- Integration
- Middleware
- Open Source
---
