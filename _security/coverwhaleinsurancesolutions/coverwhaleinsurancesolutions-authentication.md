---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coverwhaleinsurancesolutions-authentication-api-openapi.yml
  format: yaml
  label: Cover Whale Authentication API
  slug: coverwhaleinsurancesolutions-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-authentication-api-openapi.yml
- filename: coverwhaleinsurancesolutions-binding-api-openapi.yml
  format: yaml
  label: Cover Whale Binding API
  slug: coverwhaleinsurancesolutions-binding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-binding-api-openapi.yml
- filename: coverwhaleinsurancesolutions-policy-lifecycle-api-openapi.yml
  format: yaml
  label: Cover Whale Policy Lifecycle API
  slug: coverwhaleinsurancesolutions-policy-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-policy-lifecycle-api-openapi.yml
- filename: coverwhaleinsurancesolutions-quoting-api-openapi.yml
  format: yaml
  label: Cover Whale Quoting API
  slug: coverwhaleinsurancesolutions-quoting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-quoting-api-openapi.yml
- filename: coverwhaleinsurancesolutions-reference-data-api-openapi.yml
  format: yaml
  label: Cover Whale Reference Data API
  slug: coverwhaleinsurancesolutions-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-reference-data-api-openapi.yml
- filename: coverwhaleinsurancesolutions-submission-data-api-openapi.yml
  format: yaml
  label: Cover Whale Submission Data API
  slug: coverwhaleinsurancesolutions-submission-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-submission-data-api-openapi.yml
- filename: coverwhaleinsurancesolutions-submissions-api-openapi.yml
  format: yaml
  label: Cover Whale Submissions API
  slug: coverwhaleinsurancesolutions-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-submissions-api-openapi.yml
- filename: coverwhaleinsurancesolutions-webhooks-api-openapi.yml
  format: yaml
  label: Cover Whale Webhooks API
  slug: coverwhaleinsurancesolutions-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-webhooks-api-openapi.yml
auth_types: []
description: Cover Whale uses a custom API key scheme named AccessToken.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coverwhaleinsurancesolutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cover Whale declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cover Whale
provider_slug: coverwhaleinsurancesolutions
scheme_count: 1
schemes:
- evidence: 'The header name is `AccessToken` (no space, no "Bearer" prefix). This differs from the standard `Authorization: Bearer <token>` pattern.'
  header: AccessToken
  how_to_obtain: Send a POST request to https://api.coverwhale.dev/v1/authentication with a JSON body containing "username" and "password" to receive an AccessToken and RefreshToken.
  location: header
  name: AccessToken
  type: apiKey
slug: coverwhaleinsurancesolutions-authentication
source_filename: coverwhaleinsurancesolutions-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.coverwhale.com/authentication.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.coverwhale.com/authentication.md\nsources:\n- https://docs.coverwhale.com/authentication.md\n- https://docs.coverwhale.com/api-reference/authentication/check-api-health.md\n- https://docs.coverwhale.com/api-reference/authentication/get-authentication-token.md\n- https://docs.coverwhale.com/api-reference/authentication/get-a-password-reset-token.md\ndescription: Cover Whale uses a custom API key scheme named AccessToken.\nschemes:\n- type: apiKey\n  name: AccessToken\n  evidence: 'The header name is `AccessToken` (no space, no \"Bearer\" prefix). This differs from the standard `Authorization: Bearer <token>` pattern.'\n  location: header\n  header: AccessToken\n  how_to_obtain: Send a POST request to https://api.coverwhale.dev/v1/authentication with a JSON body containing \"username\" and \"password\" to\n    receive an AccessToken and RefreshToken.\ndocs: https://docs.coverwhale.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/coverwhaleinsurancesolutions/authentication/coverwhaleinsurancesolutions-authentication.yml
summary_line: 1 scheme
tags:
- Insurance
- Commercial Auto Insurance
- Insurtech
- Underwriting
- Telematics
- Risk Management
- Fleet Safety
- Policy Lifecycle
- Webhook
- Company
---
