---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kawaa-com-account-api-openapi.yml
  format: yaml
  label: kawaa-com Account API
  slug: kawaa-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-account-api-openapi.yml
- filename: kawaa-com-activity-api-openapi.yml
  format: yaml
  label: kawaa-com Activity API
  slug: kawaa-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-activity-api-openapi.yml
- filename: kawaa-com-api-keys-api-openapi.yml
  format: yaml
  label: kawaa-com API keys API
  slug: kawaa-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-api-keys-api-openapi.yml
- filename: kawaa-com-catalogue-api-openapi.yml
  format: yaml
  label: kawaa-com Catalogue API
  slug: kawaa-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-catalogue-api-openapi.yml
- filename: kawaa-com-deliverability-api-openapi.yml
  format: yaml
  label: kawaa-com Deliverability API
  slug: kawaa-com-deliverability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-deliverability-api-openapi.yml
- filename: kawaa-com-exports-api-openapi.yml
  format: yaml
  label: kawaa-com Exports API
  slug: kawaa-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-exports-api-openapi.yml
- filename: kawaa-com-health-api-openapi.yml
  format: yaml
  label: kawaa-com Health API
  slug: kawaa-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-health-api-openapi.yml
- filename: kawaa-com-jobs-api-openapi.yml
  format: yaml
  label: kawaa-com Jobs API
  slug: kawaa-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-jobs-api-openapi.yml
- filename: kawaa-com-search-api-openapi.yml
  format: yaml
  label: kawaa-com Search API
  slug: kawaa-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-search-api-openapi.yml
- filename: kawaa-com-verification-api-openapi.yml
  format: yaml
  label: kawaa-com Verification API
  slug: kawaa-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-verification-api-openapi.yml
- filename: kawaa-com-webhooks-api-openapi.yml
  format: yaml
  label: kawaa-com Webhooks API
  slug: kawaa-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for Kawaa API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kawaa Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: kawaa-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: kawaa-com
provider_slug: kawaa-com
scheme_count: 2
schemes:
- evidence: 'Include your API key in the X-Api-Key header with every request:'
  header: X-Api-Key
  how_to_obtain: Create and manage API keys in the Kawaa Dashboard
  location: header
  name: X-Api-Key
  type: apiKey
- evidence: The same key is also accepted as a bearer token, for HTTP clients that only know how to send an Authorization header.
  header: Authorization
  how_to_obtain: Create and manage API keys in the Kawaa Dashboard
  location: header
  name: Authorization
  type: http-bearer
slug: kawaa-com-authentication
source_filename: kawaa-com-authentication.yml
source_heading: Authentication Profile
source_url: https://kawaa.com/docs/api/account/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kawaa.com/docs/api/account/\nsources:\n- https://kawaa.com/docs/api/account/\n- https://kawaa.com/docs/authentication/\n- https://kawaa.com/blog/email-authentication-spf-dkim-dmarc/\n- https://kawaa.com/support/api-auth/\ndescription: Authentication methods for Kawaa API\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'Include your API key in the X-Api-Key header with every request:'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create and manage API keys in the Kawaa Dashboard\n- type: http-bearer\n  name: Authorization\n  evidence: The same key is also accepted as a bearer token, for HTTP clients that only know how to send an Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create and manage API keys in the Kawaa Dashboard\nnote: OAuth authentication is mentioned but no token or authorize URLs, flows, or scopes\
  \ are provided on the pages.\ndocs: https://kawaa.com/docs/api/account/\n"
source_yaml_url: https://artifacts.apis.io/kawaa-com/authentication/kawaa-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Email Verification
- Software-as-a-Service
- Marketing
---
