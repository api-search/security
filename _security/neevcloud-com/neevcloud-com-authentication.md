---
anonymous_access: false
api_key_in: []
api_specs:
- filename: neevcloud-com-openapi-generated.yml
  format: yaml
  label: NeevCloud API
  slug: neevcloud-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neevcloud-com/openapi/_ae-authored/neevcloud-com-openapi-generated.yml
auth_types: []
description: NeevCloud supports API key authentication via the Authorization header and bearer token authentication for user login endpoints.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: NeevCloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: NeevCloud declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: NeevCloud
provider_slug: neevcloud-com
scheme_count: 2
schemes:
- evidence: Every request you send includes this key in the Authorization header, and NeevCloud validates it before processing the request.
  header: Authorization
  how_to_obtain: Create an API key in the NeevCloud Console under Account → API Keys and copy the generated key.
  location: header
  name: API Key
  type: apiKey
- evidence: Use the **`access_token`** from `POST /api/v1/auth/login` (same credentials as the console). In **Authorize**, paste **only that token** — do not prepend `Bearer`, and do not use inference keys (`sk-nc-*`) here.
  header: Authorization
  how_to_obtain: Log in via the `/api/v1/auth/login` endpoint with email and password to receive an `access_token`.
  location: header
  name: BearerAuth
  type: http-bearer
slug: neevcloud-com-authentication
source_filename: neevcloud-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ai.neevcloud.com/getting-started/create-api-key.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ai.neevcloud.com/getting-started/create-api-key.md\nsources:\n- https://docs.ai.neevcloud.com/getting-started/create-api-key.md\n- https://docs.ai.neevcloud.com/ai-inference/overview-1/authentication.md\n- https://docs.ai.neevcloud.com/tutorials/start-here/create-api-key.md\n- https://docs.ai.neevcloud.com/api-reference/tenant/authentication.md\ndescription: NeevCloud supports API key authentication via the Authorization header and bearer token authentication for user login endpoints.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request you send includes this key in the Authorization header, and NeevCloud validates it before processing the request.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the NeevCloud Console under Account → API Keys and copy the generated key.\n- type: http-bearer\n  name: BearerAuth\n  evidence:\
  \ Use the **`access_token`** from `POST /api/v1/auth/login` (same credentials as the console). In **Authorize**, paste **only that token**\n    — do not prepend `Bearer`, and do not use inference keys (`sk-nc-*`) here.\n  location: header\n  header: Authorization\n  how_to_obtain: Log in via the `/api/v1/auth/login` endpoint with email and password to receive an `access_token`.\ndocs: https://docs.ai.neevcloud.com/getting-started/create-api-key.md\n"
source_yaml_url: https://artifacts.apis.io/neevcloud-com/authentication/neevcloud-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Cloud
- Supercloud
- GPU
- Kubernetes
---
