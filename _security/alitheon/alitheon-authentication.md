---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published by Alitheon
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Alitheon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alitheon declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Alitheon
provider_slug: alitheon
scheme_count: 1
schemes:
- evidence: The service client credentials (client id and client secret) can be used indefinitely to log in non‑interactively using the /authz/v1/token‑exchange/client endpoint described in the API documentation.
  flows:
  - client_credentials
  how_to_obtain: Create a service client in the Web Portal (User Management → New Service Client) and copy the client Id and client secret.
  name: Service Client Credential Flow
  token_url: /authz/v1/token-exchange/client
  type: oauth2
slug: alitheon-authentication
source_filename: alitheon-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.alitheon.com/docs/fp4-integration-doc/7whjca4580q0u-authentication-and-authorization
source_yaml: "generated: '2026-09-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.alitheon.com/docs/fp4-integration-doc/7whjca4580q0u-authentication-and-authorization\nsources:\n- https://docs.alitheon.com/docs/fp4-integration-doc/7whjca4580q0u-authentication-and-authorization\n- https://docs.alitheon.com/docs/user-guide/9thid5p81kyai-getting-started\ndescription: Authentication methods published by Alitheon\nschemes:\n- type: oauth2\n  name: Service Client Credential Flow\n  evidence: The service client credentials (client id and client secret) can be used indefinitely to log in non‑interactively using the /authz/v1/token‑exchange/client\n    endpoint described in the API documentation.\n  flows:\n  - client_credentials\n  token_url: /authz/v1/token-exchange/client\n  how_to_obtain: Create a service client in the Web Portal (User Management → New Service Client) and copy the client Id and client secret.\ndocs: https://docs.alitheon.com/docs/fp4-integration-doc/7whjca4580q0u-authentication-and-authorization\n\
  note: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alitheon/refs/heads/main/authentication/alitheon-authentication.yml
summary_line: 1 scheme
tags:
- Authentication
- Anti‑Counterfeit
- Asset Management
- Supply Chain
- Physical Identity
- Optical AI
---
