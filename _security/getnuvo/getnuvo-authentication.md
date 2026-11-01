---
anonymous_access: false
api_key_in: []
auth_types: []
description: The Ingestro pipeline API uses a license key to generate access tokens, which are then sent in the request header as a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Getnuvo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ingestro declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ingestro
provider_slug: getnuvo
scheme_count: 1
schemes:
- evidence: All API requests should be made over HTTPS . API requests without authentication will fail.
  header: access_token
  how_to_obtain: Generate an access token via a POST request to the token_url with a JSON body containing your license_key and an auth object (identifier and type).
  location: header
  name: Access Token
  token_url: https://api-gateway.ingestro.com/dp/api/v1/access/token
  type: http-bearer
slug: getnuvo-authentication
source_filename: getnuvo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ingestro.com/dp/authentication-api/
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ingestro.com/dp/authentication-api/\nsources:\n- https://docs.ingestro.com/dp/authentication-api/\ndescription: The Ingestro pipeline API uses a license key to generate access tokens, which are then sent in the request header as a bearer token.\nschemes:\n- type: http-bearer\n  name: Access Token\n  evidence: All API requests should be made over HTTPS . API requests without authentication will fail.\n  location: header\n  header: access_token\n  token_url: https://api-gateway.ingestro.com/dp/api/v1/access/token\n  how_to_obtain: Generate an access token via a POST request to the token_url with a JSON body containing your license_key and an auth object\n    (identifier and type).\nnote: The license key itself is sent in the request body when obtaining an access token; subsequent API calls use the returned access_token in\n  the header.\ndocs: https://docs.ingestro.com/dp/authentication-api/\n"
source_yaml_url: https://artifacts.apis.io/getnuvo/authentication/getnuvo-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Data-Operations
- Payroll
- Automation
- Integration
---
