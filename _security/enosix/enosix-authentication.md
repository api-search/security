---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enosix-search-api-openapi.yml
  format: yaml
  label: enosix Search API
  slug: enosix-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enosix/openapi/enosix-search-api-openapi.yml
auth_types: []
description: Authentication methods for enosix Connect and Link APIs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Enosix Authentication
name_suffix: Authentication
oauth_flows: []
overview: enosix declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: enosix
provider_slug: enosix
scheme_count: 3
schemes:
- evidence: Configuring this feature causes the Connect application to authorize all incoming requests have a corresponding X-API-KEY header value to the enosix__ApiKey configuration.
  header: X-API-KEY
  how_to_obtain: Set a User-Provided Variable with key enosix__ApiKey and a generated opaque token value.
  location: header
  name: API Key
  type: apiKey
- evidence: In Passthrough mode, you must attach valid SAP credentials to each API request using basic authentication headers.
  header: Authorization
  how_to_obtain: Use valid SAP user credentials (username and password) for basic auth.
  location: header
  name: Passthrough Basic Authentication
  type: http-basic
- evidence: All requests made though API/Proxies that have OpenID Auth configured will require a Bearer JWT (JSON Web Token) authentication header provided by the configured OpenID Auth provider.
  header: Authorization
  how_to_obtain: Generate a JWT from the configured OpenID provider (e.g., via Postman or Insomnia) and include it in the Authorization header.
  location: header
  name: OpenID Bearer JWT
  type: http-bearer
slug: enosix-authentication
source_filename: enosix-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.enosix.io/connect/using-the-api/api-key
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.enosix.io/connect/using-the-api/api-key\nsources:\n- https://docs.enosix.io/connect/using-the-api/api-key\n- https://docs.enosix.io/connect/using-the-api/authentication\n- https://docs.enosix.io/release/improved-named-credentials\n- https://docs.enosix.io/link/configuration/openid-auth\ndescription: Authentication methods for enosix Connect and Link APIs\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Configuring this feature causes the Connect application to authorize all incoming requests have a corresponding X-API-KEY header value\n    to the enosix__ApiKey configuration.\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Set a User-Provided Variable with key enosix__ApiKey and a generated opaque token value.\n- type: http-basic\n  name: Passthrough Basic Authentication\n  evidence: In Passthrough mode, you must attach valid SAP credentials to each\
  \ API request using basic authentication headers.\n  location: header\n  header: Authorization\n  how_to_obtain: Use valid SAP user credentials (username and password) for basic auth.\n- type: http-bearer\n  name: OpenID Bearer JWT\n  evidence: All requests made though API/Proxies that have OpenID Auth configured will require a Bearer JWT (JSON Web Token) authentication header\n    provided by the configured OpenID Auth provider.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a JWT from the configured OpenID provider (e.g., via Postman or Insomnia) and include it in the Authorization header.\nnote: Configured Connection mode does not require client‑provided credentials; it uses credentials configured on the connection.\ndocs: https://docs.enosix.io/connect/using-the-api/api-key\n"
source_yaml_url: https://artifacts.apis.io/enosix/authentication/enosix-authentication.yml
summary_line: 3 schemes
tags:
- Company
- SAP
- Artificial Intelligence
- Integration
- Workflows
---
