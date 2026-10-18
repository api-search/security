---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nice-channels-api-openapi.yml
  format: yaml
  label: NICE Channels API
  slug: nice-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-channels-api-openapi.yml
- filename: nice-contacts-api-openapi.yml
  format: yaml
  label: NICE Contacts API
  slug: nice-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-contacts-api-openapi.yml
- filename: nice-incontactapi-api-openapi.yml
  format: yaml
  label: NICE Incontactapi API
  slug: nice-incontactapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-incontactapi-api-openapi.yml
- filename: nice-perform-action-api-openapi.yml
  format: yaml
  label: NICE Perform Action API
  slug: nice-perform-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-perform-action-api-openapi.yml
- filename: nice-result-api-openapi.yml
  format: yaml
  label: NICE Result API
  slug: nice-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-result-api-openapi.yml
- filename: nice-segments-api-openapi.yml
  format: yaml
  label: NICE Segments API
  slug: nice-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-segments-api-openapi.yml
- filename: nice-status-api-openapi.yml
  format: yaml
  label: NICE Status API
  slug: nice-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-status-api-openapi.yml
- filename: nice-user-management-api-openapi.yml
  format: yaml
  label: NICE User Management API
  slug: nice-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-user-management-api-openapi.yml
- filename: nice-voice-print-status-api-openapi.yml
  format: yaml
  label: NICE Voice Print Status API
  slug: nice-voice-print-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-voice-print-status-api-openapi.yml
- filename: nice-well-known-api-openapi.yml
  format: yaml
  label: NICE .well Known API
  slug: nice-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/nice-well-known-api-openapi.yml
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
- Customer Experience
- Artificial Intelligence
- Cloud
- Integration
---
