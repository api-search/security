---
anonymous_access: false
api_key_in: []
api_specs:
- filename: serpresult-com-account-api-openapi.yml
  format: yaml
  label: serpresult-com Account API
  slug: serpresult-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-account-api-openapi.yml
- filename: serpresult-com-api-keys-api-openapi.yml
  format: yaml
  label: serpresult-com API keys API
  slug: serpresult-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-api-keys-api-openapi.yml
- filename: serpresult-com-billing-api-openapi.yml
  format: yaml
  label: serpresult-com Billing API
  slug: serpresult-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-billing-api-openapi.yml
- filename: serpresult-com-meta-api-openapi.yml
  format: yaml
  label: serpresult-com Meta API
  slug: serpresult-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-meta-api-openapi.yml
- filename: serpresult-com-search-api-openapi.yml
  format: yaml
  label: serpresult-com Search API
  slug: serpresult-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-search-api-openapi.yml
- filename: serpresult-com-usage-api-openapi.yml
  format: yaml
  label: serpresult-com Usage API
  slug: serpresult-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpresult-com/openapi/serpresult-com-usage-api-openapi.yml
auth_types: []
description: 'Public API calls send a secret key in the Authorization header:'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Serpresult Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: serpresult-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: serpresult-com
provider_slug: serpresult-com
scheme_count: 1
schemes:
- evidence: 'Public API calls send a secret key in the Authorization header: Authorization: Bearer sk_live_…'
  header: Authorization
  how_to_obtain: Keys are minted in the dashboard under Developers → API Keys and the plaintext secret is shown once on creation or rotation.
  location: header
  name: Bearer
  type: http-bearer
slug: serpresult-com-authentication
source_filename: serpresult-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.serpresult.com/api/authentication/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.serpresult.com/api/authentication/\nsources:\n- https://docs.serpresult.com/api/authentication/\n- https://docs.serpresult.com/api/quickstart/\ndescription: 'Public API calls send a secret key in the Authorization header:'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Public API calls send a secret key in the Authorization header: Authorization: Bearer sk_live_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are minted in the dashboard under Developers → API Keys and the plaintext secret is shown once on creation or rotation.\nnote: Other credentials (marketing site’s keyless demo header and RapidAPI marketplace proxy secret) exist but are not sent manually.\ndocs: https://docs.serpresult.com/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/serpresult-com/authentication/serpresult-com-authentication.yml
summary_line: 1 scheme
tags:
- SERP
- Search
- API
- Aggregator
- SEO
---
