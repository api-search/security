---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dynamo-ai-dynamo-ai-api-api-openapi.yml
  format: yaml
  label: Dynamo AI API
  slug: dynamo-ai-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamo-ai/openapi/dynamo-ai-dynamo-ai-api-api-openapi.yml
- filename: dynamo-ai-openapi-generated.yml
  format: yaml
  label: Dynamo AI API
  slug: dynamo-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamo-ai/openapi/_ae-authored/dynamo-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for Dynamo AI as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dynamo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamo AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dynamo AI
provider_slug: dynamo-ai
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://API_HOSTNAME/v1/user/token \ -H "Authorization: Bearer CURRENT_API_KEY"'
  header: Authorization
  how_to_obtain: Obtain a new API key by calling the token endpoint with an existing API key.
  location: header
  name: Platform API Key
  type: http-bearer
slug: dynamo-ai-authentication
source_filename: dynamo-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dynamo.ai/docs/Onboarding/IAM/Rotating-Credentials
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dynamo.ai/docs/Onboarding/IAM/Rotating-Credentials\nsources:\n- https://docs.dynamo.ai/docs/Onboarding/IAM/Rotating-Credentials\n- https://docs.dynamo.ai/docs/Operations/Upgrades/redis-auth-tls-migration\n- https://docs.dynamo.ai/docs/sdk-reference/usage/user-auth\n- https://docs.dynamo.ai/docs/DynamoEval/Getting%20started/Quickstart%20-%20Jailbreaking/jailbreak-sdk-quickstart\ndescription: Authentication schemes for Dynamo AI as documented.\nschemes:\n- type: http-bearer\n  name: Platform API Key\n  evidence: 'curl -X POST https://API_HOSTNAME/v1/user/token \\ -H \"Authorization: Bearer CURRENT_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a new API key by calling the token endpoint with an existing API key.\ndocs: https://docs.dynamo.ai/docs/Onboarding/IAM/Rotating-Credentials\n"
source_yaml_url: https://artifacts.apis.io/dynamo-ai/authentication/dynamo-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Security
- Enterprise
- Compliance
---
