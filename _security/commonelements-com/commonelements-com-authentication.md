---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commonelements-com-aggregates-and-compliance-api-openapi.yml
  format: yaml
  label: Common Elements Aggregates and compliance API
  slug: commonelements-com-aggregates-and-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-aggregates-and-compliance-api-openapi.yml
- filename: commonelements-com-association-resources-api-openapi.yml
  format: yaml
  label: Common Elements Association resources API
  slug: commonelements-com-association-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-association-resources-api-openapi.yml
- filename: commonelements-com-associations-api-openapi.yml
  format: yaml
  label: Common Elements Associations API
  slug: commonelements-com-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-associations-api-openapi.yml
- filename: commonelements-com-bulk-delivery-api-openapi.yml
  format: yaml
  label: Common Elements Bulk delivery API
  slug: commonelements-com-bulk-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-bulk-delivery-api-openapi.yml
- filename: commonelements-com-bulk-export-api-openapi.yml
  format: yaml
  label: Common Elements Bulk export API
  slug: commonelements-com-bulk-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-bulk-export-api-openapi.yml
- filename: commonelements-com-change-feed-api-openapi.yml
  format: yaml
  label: Common Elements Change feed API
  slug: commonelements-com-change-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-change-feed-api-openapi.yml
- filename: commonelements-com-cross-association-collections-api-openapi.yml
  format: yaml
  label: Common Elements Cross-association collections API
  slug: commonelements-com-cross-association-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-cross-association-collections-api-openapi.yml
- filename: commonelements-com-dataset-catalog-api-openapi.yml
  format: yaml
  label: Common Elements Dataset catalog API
  slug: commonelements-com-dataset-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-dataset-catalog-api-openapi.yml
- filename: commonelements-com-meta-api-openapi.yml
  format: yaml
  label: Common Elements Meta API
  slug: commonelements-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-meta-api-openapi.yml
- filename: commonelements-com-professionals-and-licenses-api-openapi.yml
  format: yaml
  label: Common Elements Professionals and licenses API
  slug: commonelements-com-professionals-and-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-professionals-and-licenses-api-openapi.yml
- filename: commonelements-com-statutes-api-openapi.yml
  format: yaml
  label: Common Elements Statutes API
  slug: commonelements-com-statutes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-statutes-api-openapi.yml
- filename: commonelements-com-vendors-api-openapi.yml
  format: yaml
  label: Common Elements Vendors API
  slug: commonelements-com-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-vendors-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Common Elements Authentication
name_suffix: Authentication
oauth_flows: []
overview: Common Elements secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Common Elements
provider_slug: commonelements-com
scheme_count: 1
schemes:
- description: 'An API key from /settings/api-keys, sent as `Authorization: Bearer ce_live_...`. Sandbox requests use the published test key documented at /api/v1/meta/sandbox.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/commonelements-com-openapi.yml
  type: http
slug: commonelements-com-authentication
source_filename: commonelements-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commonelements.com/developers/docs/getting-started\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API key from /settings/api-keys, sent as `Authorization: Bearer\n    ce_live_...`. Sandbox requests use the published test key documented at /api/v1/meta/sandbox.'\n  sources:\n  - openapi/commonelements-com-openapi.yml\ndocs: https://commonelements.com/developers/docs/getting-started\nkey_management:\n  issue: Settings -> API keys (/settings/api-keys); raw key shown exactly once\n  prefixes:\n    live: ce_live_\n    sandbox: ce_test_sandbox (public, sandbox only)\n  ownership: Personal or organization keys; a key inherits the owner plan\n  rotation: Revoke and create a new key; no way to reveal a raw key a second time\n  scopes: Per-key resource scopes, see scopes/commonelements-com-scopes.yml\nmcp_auth:\n  endpoint: https://commonelements.com/api/mcp\n \
  \ method: 'OAuth sign-in with a Common Elements account (read/write grants split per\n    domain, read-only default); JSON-config clients may send Authorization: Bearer\n    ce_live_...'\n  source: https://commonelements.com/developers/mcp\n"
source_yaml_url: https://artifacts.apis.io/commonelements-com/authentication/commonelements-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- HOA
- Community Associations
- Real Estate
- PropTech
- Property Data
- Compliance
- Flood Risk
---
