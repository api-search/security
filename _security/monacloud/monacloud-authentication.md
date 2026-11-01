---
anonymous_access: false
api_key_in: []
api_specs:
- filename: monacloud-apps-api-openapi.yml
  format: yaml
  label: The MONA Group Apps API
  slug: monacloud-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-apps-api-openapi.yml
- filename: monacloud-auth-api-openapi.yml
  format: yaml
  label: The MONA Group Auth API
  slug: monacloud-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-auth-api-openapi.yml
- filename: monacloud-billing-api-openapi.yml
  format: yaml
  label: The MONA Group Billing API
  slug: monacloud-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-billing-api-openapi.yml
- filename: monacloud-databases-api-openapi.yml
  format: yaml
  label: The MONA Group Databases API
  slug: monacloud-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-databases-api-openapi.yml
- filename: monacloud-jobs-api-openapi.yml
  format: yaml
  label: The MONA Group Jobs API
  slug: monacloud-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-jobs-api-openapi.yml
- filename: monacloud-lxc-api-openapi.yml
  format: yaml
  label: The MONA Group Lxc API
  slug: monacloud-lxc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-lxc-api-openapi.yml
- filename: monacloud-prices-api-openapi.yml
  format: yaml
  label: The MONA Group Prices API
  slug: monacloud-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-prices-api-openapi.yml
- filename: monacloud-sandbox-api-openapi.yml
  format: yaml
  label: The MONA Group Sandbox API
  slug: monacloud-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-sandbox-api-openapi.yml
- filename: monacloud-services-api-openapi.yml
  format: yaml
  label: The MONA Group Services API
  slug: monacloud-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monacloud/openapi/monacloud-services-api-openapi.yml
auth_types: []
description: Authentication methods described in the MONA Cloud documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Monacloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: The MONA Group declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: The MONA Group
provider_slug: monacloud
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer $MONACLOUD_TOKEN"'
  header: Authorization
  how_to_obtain: Create an API key via POST /api/api-keys; the response contains the token to use as a Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: monacloud-authentication
source_filename: monacloud-authentication.yml
source_heading: Authentication Profile
source_url: https://monacloud.vn/docs/bao-mat
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://monacloud.vn/docs/bao-mat\nsources:\n- https://monacloud.vn/docs/bao-mat\n- https://monacloud.vn/en/docs/quick-start\n- https://monacloud.vn/en/docs/quick-start.md\n- https://monacloud.vn/en/docs/quick-start.txt\ndescription: Authentication methods described in the MONA Cloud documentation.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '-H \"Authorization: Bearer $MONACLOUD_TOKEN\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via POST /api/api-keys; the response contains the token to use as a Bearer token.\ndocs: https://monacloud.vn/docs/bao-mat\n"
source_yaml_url: https://artifacts.apis.io/monacloud/authentication/monacloud-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- Hosting
- Developer Tools
- Vietnamese
- Artificial Intelligence
---
