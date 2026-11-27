---
anonymous_access: false
api_key_in: []
api_specs:
- filename: databend-openapi-generated.yml
  format: yaml
  label: Databend API
  slug: databend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databend/openapi/_ae-authored/databend-openapi-generated.yml
auth_types: []
description: Key‑pair authentication uses a JWT signed with the client’s private key, sent as a Bearer token together with a custom header that selects the key‑pair flow.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Databend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Databend declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Databend
provider_slug: databend
scheme_count: 1
schemes:
- evidence: 'The client generates a short-lived JWT signed with the private key and sends it as a Bearer token with a custom header to distinguish from JWKS-based JWT auth:'
  header: Authorization
  how_to_obtain: 'Generate a short‑lived JWT signed with the user''s private key; include it in the Authorization: Bearer <jwt_token> header and add X-DATABEND-AUTH-METHOD: keypair header.'
  location: header
  name: keypair
  type: http-bearer
slug: databend-authentication
source_filename: databend-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.databend.com/developer/community/rfcs/key-pair-auth
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.databend.com/developer/community/rfcs/key-pair-auth\nsources:\n- https://docs.databend.com/developer/community/rfcs/key-pair-auth\n- https://docs.databend.com/guides/cloud/getting-started.md\n- https://docs.databend.com/guides/cloud/getting-started\n- https://docs.databend.com/guides/self-hosted/deployment/production/benddeploy/getting-started\ndescription: Key‑pair authentication uses a JWT signed with the client’s private key, sent as a Bearer token together with a custom header that\n  selects the key‑pair flow.\nschemes:\n- type: http-bearer\n  name: keypair\n  evidence: 'The client generates a short-lived JWT signed with the private key and sends it as a Bearer token with a custom header to distinguish\n    from JWKS-based JWT auth:'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Generate a short‑lived JWT signed with the user''s private key; include\
  \ it in the Authorization: Bearer <jwt_token> header and\n    add X-DATABEND-AUTH-METHOD: keypair header.'\nnote: 'The X-DATABEND-AUTH-METHOD: keypair header is required in addition to the Authorization Bearer header.'\ndocs: https://docs.databend.com/developer/community/rfcs/key-pair-auth\n"
source_yaml_url: https://artifacts.apis.io/databend/authentication/databend-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data Warehouse
- Cloud
- Open Source
- Analytics
---
