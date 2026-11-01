---
anonymous_access: false
api_key_in: []
api_specs:
- filename: writestack-openapi-generated.yml
  format: yaml
  label: WriteStack API
  slug: writestack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/writestack/openapi/_ae-authored/writestack-openapi-generated.yml
auth_types: []
description: Vercel authenticates API and CLI requests using personal access tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Writestack Authentication
name_suffix: Authentication
oauth_flows: []
overview: WriteStack declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: WriteStack
provider_slug: writestack
scheme_count: 1
schemes:
- evidence: Pass the token as a Bearer token in the `Authorization` header of your request.
  header: Authorization
  how_to_obtain: Create a token in the Vercel dashboard under Account Tokens, or via the REST API or Vercel CLI (`vercel tokens create`).
  location: header
  name: Vercel Access Token
  type: http-bearer
slug: writestack-authentication
source_filename: writestack-authentication.yml
source_heading: Authentication Profile
source_url: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\nsources:\n- https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\n- https://vercel.com/docs/cli/tokens.md\n- https://vercel.com/docs/getting-started-with-vercel.md?from=llms-txt\ndescription: Vercel authenticates API and CLI requests using personal access tokens.\nschemes:\n- type: http-bearer\n  name: Vercel Access Token\n  evidence: Pass the token as a Bearer token in the `Authorization` header of your request.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in the Vercel dashboard under Account Tokens, or via the REST API or Vercel CLI (`vercel tokens create`).\ndocs: https://vercel.com/docs/accounts/access-tokens.md#use-a-scoped-token-with-the-api\n"
source_yaml_url: https://artifacts.apis.io/writestack/authentication/writestack-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Substack
- Growth
- Analytics
- ContentCreation
---
