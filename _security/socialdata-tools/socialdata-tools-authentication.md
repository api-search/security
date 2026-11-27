---
anonymous_access: false
api_key_in: []
api_specs:
- filename: socialdata-tools-data-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Data API
  slug: socialdata-tools-data-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-data-api-api-openapi.yml
- filename: socialdata-tools-monitoring-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Monitoring API
  slug: socialdata-tools-monitoring-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-monitoring-api-api-openapi.yml
- filename: socialdata-tools-social-actions-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Social Actions API
  slug: socialdata-tools-social-actions-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-social-actions-api-api-openapi.yml
- filename: socialdata-tools-socialdata-account-management-api-openapi.yml
  format: yaml
  label: socialdata-tools SocialData Account Management API
  slug: socialdata-tools-socialdata-account-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-socialdata-account-management-api-openapi.yml
auth_types: []
description: Authentication using an API key sent in the Authorization header as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: socialdata-tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: socialdata-tools declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: socialdata-tools
provider_slug: socialdata-tools
scheme_count: 1
schemes:
- evidence: 'Include your API key as `Authorization: Bearer YOUR_API_KEY` header with all requests'
  header: Authorization
  how_to_obtain: Generate your API key in your user dashboard after signing up.
  location: header
  name: API Key
  type: apiKey
slug: socialdata-tools-authentication
source_filename: socialdata-tools-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.socialdata.tools/getting-started/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.socialdata.tools/getting-started/authentication.md\nsources:\n- https://docs.socialdata.tools/getting-started/authentication.md\n- https://docs.socialdata.tools/getting-started/overview.md\n- https://docs.socialdata.tools/getting-started/pricing.md\n- https://docs.socialdata.tools/getting-started/rate-limits.md\ndescription: Authentication using an API key sent in the Authorization header as a Bearer token.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Include your API key as `Authorization: Bearer YOUR_API_KEY` header with all requests'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate your API key in your user dashboard after signing up.\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://docs.socialdata.tools/getting-started/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/socialdata-tools/authentication/socialdata-tools-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Media
- Data
- Public APIs
---
