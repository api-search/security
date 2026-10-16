---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fused-openapi-generated.yml
  format: yaml
  label: Fused API
  slug: fused-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fused/refs/heads/main/openapi/_ae-authored/fused-openapi-generated.yml
auth_types: []
description: Authentication methods for Fused UDF API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fused Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fused declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Fused
provider_slug: fused
scheme_count: 2
schemes:
- evidence: Add the session token as a fused_session_token query parameter on the UDF HTTPS URL (same host and path as a normal canvas call, for example https://udf.ai/fc_<CANVAS_TOKEN>/<udf_name>.json).
  how_to_obtain: Mint a session token via the Fused Service Account using the POST /session-token/by-access-token/{canvas_token} endpoint.
  location: query
  name: fused_session_token
  type: apiKey
- evidence: 'Calling UDFs with Bearer authentication requires an account''s private token . curl -XGET "https://udf.ai/fc_YOUR_CANVAS_TOKEN/my_udf.png" -H "Authorization: Bearer $ACCESS_TOKEN "'
  header: 'Authorization: Bearer <TOKEN>'
  how_to_obtain: Retrieve your bearer token via the fused._auth library or your account settings.
  location: header
  name: Authorization
  type: http-bearer
slug: fused-authentication
source_filename: fused-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fused.io/guide/data-input-outputs/export-api/securing-shared-tokens/
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fused.io/guide/data-input-outputs/export-api/securing-shared-tokens/\nsources:\n- https://docs.fused.io/guide/data-input-outputs/export-api/securing-shared-tokens/\n- https://docs.fused.io/guide/data-input-outputs/export-api/tokens-endpoints/\n- https://docs.fused.io/rest-api/tokens/\n- https://docs.fused.io/guide/advanced-setup/dependencies/\ndescription: Authentication methods for Fused UDF API\nschemes:\n- type: apiKey\n  name: fused_session_token\n  evidence: Add the session token as a fused_session_token query parameter on the UDF HTTPS URL (same host and path as a normal canvas call, for\n    example https://udf.ai/fc_<CANVAS_TOKEN>/<udf_name>.json).\n  location: query\n  how_to_obtain: Mint a session token via the Fused Service Account using the POST /session-token/by-access-token/{canvas_token} endpoint.\n- type: http-bearer\n  name: Authorization\n  evidence:\
  \ 'Calling UDFs with Bearer authentication requires an account''s private token . curl -XGET \"https://udf.ai/fc_YOUR_CANVAS_TOKEN/my_udf.png\"\n    -H \"Authorization: Bearer $ACCESS_TOKEN \"'\n  location: header\n  header: 'Authorization: Bearer <TOKEN>'\n  how_to_obtain: Retrieve your bearer token via the fused._auth library or your account settings.\ndocs: https://docs.fused.io/guide/data-input-outputs/export-api/securing-shared-tokens/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fused/refs/heads/main/authentication/fused-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Analytics
- AI
- DataPlatform
- Python
- LowCode
---
