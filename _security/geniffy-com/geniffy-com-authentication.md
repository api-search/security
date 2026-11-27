---
anonymous_access: false
api_key_in: []
api_specs:
- filename: geniffy-com-account-api-openapi.yml
  format: yaml
  label: Geniffy Account API
  slug: geniffy-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-account-api-openapi.yml
- filename: geniffy-com-admin-api-openapi.yml
  format: yaml
  label: Geniffy Admin API
  slug: geniffy-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-admin-api-openapi.yml
- filename: geniffy-com-developer-api-api-openapi.yml
  format: yaml
  label: Geniffy Developer API
  slug: geniffy-com-developer-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-developer-api-api-openapi.yml
- filename: geniffy-com-docs-api-openapi.yml
  format: yaml
  label: Geniffy Docs API
  slug: geniffy-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-docs-api-openapi.yml
- filename: geniffy-com-genify-backend-api-openapi.yml
  format: yaml
  label: Geniffy Genify Backend API
  slug: geniffy-com-genify-backend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-genify-backend-api-openapi.yml
- filename: geniffy-com-health-api-openapi.yml
  format: yaml
  label: Geniffy Health API
  slug: geniffy-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-health-api-openapi.yml
- filename: geniffy-com-infrastructure-api-openapi.yml
  format: yaml
  label: Geniffy Infrastructure API
  slug: geniffy-com-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-infrastructure-api-openapi.yml
- filename: geniffy-com-memory-app-api-openapi.yml
  format: yaml
  label: Geniffy Memory app API
  slug: geniffy-com-memory-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-memory-app-api-openapi.yml
- filename: geniffy-com-payments-api-openapi.yml
  format: yaml
  label: Geniffy Payments API
  slug: geniffy-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-payments-api-openapi.yml
- filename: geniffy-com-support-api-openapi.yml
  format: yaml
  label: Geniffy Support API
  slug: geniffy-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-support-api-openapi.yml
- filename: geniffy-com-users-api-openapi.yml
  format: yaml
  label: Geniffy Users API
  slug: geniffy-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-users-api-openapi.yml
- filename: geniffy-com-waitlist-api-openapi.yml
  format: yaml
  label: Geniffy Waitlist API
  slug: geniffy-com-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniffy-com/openapi/geniffy-com-waitlist-api-openapi.yml
auth_types: []
description: Authentication uses an API key passed in the X-Geniffy-Space header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Geniffy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geniffy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Geniffy
provider_slug: geniffy-com
scheme_count: 1
schemes:
- evidence: '`X-Geniffy-Space` | header | string | One of your own users, for every call this client makes.'
  header: X-Geniffy-Space
  how_to_obtain: Create a key via POST /v1/keys and use the returned `key` value as the X-Geniffy-Space header.
  location: header
  name: X-Geniffy-Space
  type: apiKey
slug: geniffy-com-authentication
source_filename: geniffy-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.geniffy.com/api/keys.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.geniffy.com/api/keys.md\nsources:\n- https://docs.geniffy.com/api/keys.md\n- https://docs.geniffy.com/api/key.md\n- https://docs.geniffy.com/api/keys\n- https://docs.geniffy.com/api/key\ndescription: Authentication uses an API key passed in the X-Geniffy-Space header.\nschemes:\n- type: apiKey\n  name: X-Geniffy-Space\n  evidence: '`X-Geniffy-Space` | header | string | One of your own users, for every call this client makes.'\n  location: header\n  header: X-Geniffy-Space\n  how_to_obtain: Create a key via POST /v1/keys and use the returned `key` value as the X-Geniffy-Space header.\ndocs: https://docs.geniffy.com/api/keys.md\n"
source_yaml_url: https://artifacts.apis.io/geniffy-com/authentication/geniffy-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Infrastructure
- Platform
- Enterprise
---
