---
anonymous_access: false
api_key_in: []
api_specs:
- filename: docuwriter-ai-well-known-openapi.json
  format: json
  label: DocuWriter.ai REST API .well-known API
  slug: docuwriter-ai-rest-api-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuwriter-ai/openapi/_original/docuwriter-ai-well-known-openapi.json
auth_types: []
description: Bearer token authentication using the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DocuWriter.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocuWriter.ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DocuWriter.ai
provider_slug: docuwriter-ai
scheme_count: 1
schemes:
- evidence: 'Copy the newly issued token into server-side secret storage and send it using the Authorization header:'
  header: Authorization
  how_to_obtain: Sign in and open Settings → API Tokens to create a token.
  location: header
  name: Bearer
  type: http-bearer
slug: docuwriter-ai-authentication
source_filename: docuwriter-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.docuwriter.ai/docuwriterai-api-docs/api-reference/start-with-the-api/bearer-authentication-and-token-management
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.docuwriter.ai/docuwriterai-api-docs/api-reference/start-with-the-api/bearer-authentication-and-token-management\nsources:\n- https://docs.docuwriter.ai/docuwriterai-api-docs/api-reference/start-with-the-api/bearer-authentication-and-token-management\n- https://www.docuwriter.ai/start\n- https://www.docuwriter.ai/solutions/developer-onboarding\n- https://docs.docuwriter.ai/docuwriterai-api-docs/api-reference/start-with-the-api/public-api-quickstart\ndescription: Bearer token authentication using the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Copy the newly issued token into server-side secret storage and send it using the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in and open Settings → API Tokens to create a token.\ndocs: https://docs.docuwriter.ai/docuwriterai-api-docs/api-reference/start-with-the-api/bearer-authentication-and-token-management\n"
source_yaml_url: https://artifacts.apis.io/docuwriter-ai/authentication/docuwriter-ai-authentication.yml
summary_line: 1 scheme
tags:
- Documentation
- Fintech
- Insurance
- MSP
---
