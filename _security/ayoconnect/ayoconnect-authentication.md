---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ayoconnect-bill-api-openapi.yml
  format: yaml
  label: Ayoconnect Bill API
  slug: ayoconnect-bill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayoconnect/openapi/ayoconnect-bill-api-openapi.yml
auth_types: []
description: Authentication methods for Ayoconnect APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ayoconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ayoconnect declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ayoconnect
provider_slug: ayoconnect
scheme_count: 1
schemes:
- evidence: This API is used to generate an 'Access Token,' which will be passed later in the header with the 'Authorization' key to other API calls.
  flows:
  - client_credentials
  - authorization_code
  how_to_obtain: Send a POST request with body parameter grantType and additionalInfo object; include headers X-TIMESTAMP, X-CLIENT-KEY, and X-SIGNATURE as required.
  name: B2B Access Token
  token_url: https://sandbox.api.of.ayoconnect.id/api/v3.0/access-token/b2b
  type: oauth2
slug: ayoconnect-authentication
source_filename: ayoconnect-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.payments.of.ayoconnect.id/reference/post_v1-oauth-client-credential-accesstoken
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.payments.of.ayoconnect.id/reference/post_v1-oauth-client-credential-accesstoken\nsources:\n- https://docs.payments.of.ayoconnect.id/reference/post_v1-oauth-client-credential-accesstoken\n- https://docs.ayoconnect.id/docs/token-generation.md\n- https://docs.payments.of.ayoconnect.id/reference/av-access-token-b2b\n- https://docs.payments.of.ayoconnect.id/reference/dd-v3-access-token-b2b\ndescription: Authentication methods for Ayoconnect APIs\nschemes:\n- type: oauth2\n  name: B2B Access Token\n  evidence: This API is used to generate an 'Access Token,' which will be passed later in the header with the 'Authorization' key to other API\n    calls.\n  flows:\n  - client_credentials\n  - authorization_code\n  token_url: https://sandbox.api.of.ayoconnect.id/api/v3.0/access-token/b2b\n  how_to_obtain: Send a POST request with body parameter grantType and additionalInfo object;\
  \ include headers X-TIMESTAMP, X-CLIENT-KEY, and X-SIGNATURE\n    as required.\ndocs: https://docs.payments.of.ayoconnect.id/reference/post_v1-oauth-client-credential-accesstoken\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/ayoconnect/authentication/ayoconnect-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Fintech
- Indonesia
---
