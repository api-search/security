---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getclarity-ai-media-statement-api-openapi.yml
  format: yaml
  label: Clarity Media Statement API
  slug: getclarity-ai-media-statement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclarity-ai/openapi/getclarity-ai-media-statement-api-openapi.yml
- filename: getclarity-ai-users-api-openapi.yml
  format: yaml
  label: Clarity Users API
  slug: getclarity-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclarity-ai/openapi/getclarity-ai-users-api-openapi.yml
auth_types: []
description: Authentication methods for Clarity API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Getclarity Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clarity declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clarity
provider_slug: getclarity-ai
scheme_count: 2
schemes:
- evidence: Sending a GET request with basic authentication
  header: Authorization
  how_to_obtain: Provide your CLARITY_API_USERNAME and CLARITY_API_PASSWORD as HTTP Basic credentials to the /users/token endpoint.
  location: header
  name: basicAuth
  token_url: https://api.getclarity.ai/v1/users/token
  type: http-basic
- evidence: To utilize the access token, include an `Authorization` header in your request with the format `Bearer <ACCESS_TOKEN>`.
  header: Authorization
  how_to_obtain: First obtain a JWT access token via the /users/token endpoint, then include it as a Bearer token in the Authorization header for all subsequent API calls.
  location: header
  name: Bearer JWT
  type: http-bearer
slug: getclarity-ai-authentication
source_filename: getclarity-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://clarityai.readme.io/reference/user_login_v1_token_post.md
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://clarityai.readme.io/reference/user_login_v1_token_post.md\nsources:\n- https://clarityai.readme.io/reference/user_login_v1_token_post.md\n- https://docs.getclarity.ai/reference/user_login_v1_token_post\n- https://clarityai.readme.io/reference/getting-started.md\n- https://docs.getclarity.ai/reference/getting-started\ndescription: Authentication methods for Clarity API\nschemes:\n- type: http-basic\n  name: basicAuth\n  evidence: Sending a GET request with basic authentication\n  location: header\n  header: Authorization\n  token_url: https://api.getclarity.ai/v1/users/token\n  how_to_obtain: Provide your CLARITY_API_USERNAME and CLARITY_API_PASSWORD as HTTP Basic credentials to the /users/token endpoint.\n- type: http-bearer\n  name: Bearer JWT\n  evidence: To utilize the access token, include an `Authorization` header in your request with the format `Bearer <ACCESS_TOKEN>`.\n\
  \  location: header\n  header: Authorization\n  how_to_obtain: First obtain a JWT access token via the /users/token endpoint, then include it as a Bearer token in the Authorization header\n    for all subsequent API calls.\ndocs: https://clarityai.readme.io/reference/user_login_v1_token_post.md\n"
source_yaml_url: https://artifacts.apis.io/getclarity-ai/authentication/getclarity-ai-authentication.yml
summary_line: 2 schemes
tags:
- Hiring fraud
- Identity verification
- Deepfake detection
- Talent acquisition security
- AI hiring security
---
