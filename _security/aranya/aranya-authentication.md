---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aranya-openapi-generated.yml
  format: yaml
  label: Aranya API
  slug: aranya-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aranya/openapi/_ae-authored/aranya-openapi-generated.yml
auth_types: []
description: Vercel authenticates API and CLI requests using personal access tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aranya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aranya declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aranya
provider_slug: aranya
scheme_count: 1
schemes:
- evidence: Pass the token as a Bearer token in the `Authorization` header of your request.
  header: Authorization
  how_to_obtain: Create a token on the Account Tokens page in the Vercel dashboard or via the REST API or CLI.
  location: header
  name: Vercel access token
  type: http-bearer
slug: aranya-authentication
source_filename: aranya-authentication.yml
source_heading: Authentication Profile
source_url: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\nsources:\n- https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\n- https://vercel.com/docs/cli/tokens.md\n- https://vercel.com/docs/getting-started-with-vercel.md?from=llms-txt\ndescription: Vercel authenticates API and CLI requests using personal access tokens.\nschemes:\n- type: http-bearer\n  name: Vercel access token\n  evidence: Pass the token as a Bearer token in the `Authorization` header of your request.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token on the Account Tokens page in the Vercel dashboard or via the REST API or CLI.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented on the provided pages.\ndocs: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\n"
source_yaml_url: https://artifacts.apis.io/aranya/authentication/aranya-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Infrastructure
- Cloud
- Edge
- Automation
---
