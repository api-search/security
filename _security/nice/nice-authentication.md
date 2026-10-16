---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nice-openapi-generated.yml
  format: yaml
  label: NICE API
  slug: nice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/_ae-authored/nice-openapi-generated.yml
auth_types: []
description: CXone authentication is based on OAuth 2 and OpenID Connect. Back‑end apps use standard OAuth2.0 authentication and client‑side apps use OpenID Connect.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nice Authentication
name_suffix: Authentication
oauth_flows: []
overview: NICE declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NICE
provider_slug: nice
scheme_count: 1
schemes:
- evidence: CXone authentication is based on OAuth 2 and OpenID Connect.
  flows:
  - client_credentials
  - authorization_code
  how_to_obtain: After submitting the Application Registration form, NICE provides a client_id and client_secret that are used for authentication calls.
  name: OAuth 2.0 / OpenID Connect
  type: oauth2
slug: nice-authentication
source_filename: nice-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.niceincontact.com/API/AuthenticationAPI
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.niceincontact.com/API/AuthenticationAPI\nsources:\n- https://developer.niceincontact.com/API/AuthenticationAPI\n- https://developer.niceincontact.com/Documentation/GettingStarted\ndescription: CXone authentication is based on OAuth 2 and OpenID Connect. Back‑end apps use standard OAuth2.0 authentication and client‑side apps\n  use OpenID Connect.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 / OpenID Connect\n  evidence: CXone authentication is based on OAuth 2 and OpenID Connect.\n  flows:\n  - client_credentials\n  - authorization_code\n  how_to_obtain: After submitting the Application Registration form, NICE provides a client_id and client_secret that are used for authentication\n    calls.\ndocs: https://developer.niceincontact.com/API/AuthenticationAPI\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/authentication/nice-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CustomerExperience
- AI
- Cloud
- Integration
---
