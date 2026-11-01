---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getdynamiq-api-reference-openapi-generated.yml
  format: yaml
  label: Dynamiq API Reference API
  slug: api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getdynamiq/openapi/_ae-authored/getdynamiq-api-reference-openapi-generated.yml
- filename: getdynamiq-platform-openapi-generated.yml
  format: yaml
  label: Dynamiq Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getdynamiq/openapi/_ae-authored/getdynamiq-platform-openapi-generated.yml
auth_types: []
description: Dynamiq uses bearer token authentication for both Access Keys and Personal Access Tokens.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Getdynamiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamiq declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dynamiq
provider_slug: getdynamiq
scheme_count: 2
schemes:
- evidence: 'Both are sent the same way: Authorization: Bearer <credential>'
  header: Authorization
  how_to_obtain: Create an Access Key in the UI under Settings → Access Keys or via the API (POST /v1/access-keys). The key value is shown once at creation.
  location: header
  name: Access Key
  type: http-bearer
- evidence: 'Every API request authenticates with a bearer token: curl "https://api.getdynamiq.ai/v1/apps?project_id= $PROJECT_ID " \ -H "Authorization: Bearer $DYNAMIQ_PAT "'
  header: Authorization
  how_to_obtain: Create a Personal Access Token in the UI under your profile settings → Personal access tokens, or via the API (POST /v1/personal-access-tokens). The token is shown once at creation.
  location: header
  name: Personal Access Token
  type: http-bearer
slug: getdynamiq-authentication
source_filename: getdynamiq-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.getdynamiq.ai/docs/api-reference/authentication
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.getdynamiq.ai/docs/api-reference/authentication\nsources:\n- https://docs.getdynamiq.ai/docs/api-reference/authentication\n- https://docs.getdynamiq.ai/docs/platform/administration/api-keys-and-tokens\n- https://docs.getdynamiq.ai/docs/platform/deployments/monitoring-history-and-traces\n- https://docs.getdynamiq.ai/docs/platform/get-started/quickstart-deploy-and-call\ndescription: Dynamiq uses bearer token authentication for both Access Keys and Personal Access Tokens.\nschemes:\n- type: http-bearer\n  name: Access Key\n  evidence: 'Both are sent the same way: Authorization: Bearer <credential>'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an Access Key in the UI under Settings → Access Keys or via the API (POST /v1/access-keys). The key value is shown once\n    at creation.\n- type: http-bearer\n  name: Personal Access Token\n  evidence: 'Every\
  \ API request authenticates with a bearer token: curl \"https://api.getdynamiq.ai/v1/apps?project_id= $PROJECT_ID \" \\ -H \"Authorization:\n    Bearer $DYNAMIQ_PAT \"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Personal Access Token in the UI under your profile settings → Personal access tokens, or via the API (POST /v1/personal-access-tokens).\n    The token is shown once at creation.\ndocs: https://docs.getdynamiq.ai/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/getdynamiq/authentication/getdynamiq-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Enterprise
- Platform
- Agents
---
