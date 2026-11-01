---
anonymous_access: false
api_key_in: []
api_specs:
- filename: musical-ai-openapi-generated.yml
  format: yaml
  label: Musical AI API
  slug: musical-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musical-ai/openapi/_ae-authored/musical-ai-openapi-generated.yml
auth_types: []
description: Authentication for Vercel API and CLI uses personal access tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Musical Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Musical AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Musical AI
provider_slug: musical-ai
scheme_count: 1
schemes:
- evidence: Pass the token as a Bearer token in the `Authorization` header of your request.
  header: Authorization
  how_to_obtain: Create a token on the Account Tokens page in the Vercel dashboard or via the REST API or CLI.
  location: header
  name: Vercel Access Token
  type: http-bearer
slug: musical-ai-authentication
source_filename: musical-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\nsources:\n- https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\n- https://vercel.com/docs/cli/tokens.md\n- https://vercel.com/docs/getting-started-with-vercel.md?from=llms-txt\ndescription: Authentication for Vercel API and CLI uses personal access tokens.\nschemes:\n- type: http-bearer\n  name: Vercel Access Token\n  evidence: Pass the token as a Bearer token in the `Authorization` header of your request.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token on the Account Tokens page in the Vercel dashboard or via the REST API or CLI.\nnote: Vercel does not use OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes for API authentication.\ndocs: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\n"
source_yaml_url: https://artifacts.apis.io/musical-ai/authentication/musical-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Music
- AI
- Attribution
- RightsManagement
- GenerativeAI
---
