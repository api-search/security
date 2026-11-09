---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apiosk-com-ask-api-openapi.yml
  format: yaml
  label: Apiosk Ask API
  slug: apiosk-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-ask-api-openapi.yml
- filename: apiosk-com-asks-api-openapi.yml
  format: yaml
  label: Apiosk Asks API
  slug: apiosk-com-asks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-asks-api-openapi.yml
- filename: apiosk-com-balance-api-openapi.yml
  format: yaml
  label: Apiosk Balance API
  slug: apiosk-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-balance-api-openapi.yml
- filename: apiosk-com-capabilities-api-openapi.yml
  format: yaml
  label: Apiosk Capabilities API
  slug: apiosk-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-capabilities-api-openapi.yml
- filename: apiosk-com-execute-api-openapi.yml
  format: yaml
  label: Apiosk Execute API
  slug: apiosk-com-execute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-execute-api-openapi.yml
- filename: apiosk-com-health-api-openapi.yml
  format: yaml
  label: Apiosk Health API
  slug: apiosk-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-health-api-openapi.yml
- filename: apiosk-com-runs-api-openapi.yml
  format: yaml
  label: Apiosk Runs API
  slug: apiosk-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-runs-api-openapi.yml
- filename: apiosk-com-source-readiness-api-openapi.yml
  format: yaml
  label: Apiosk Source Readiness API
  slug: apiosk-com-source-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-source-readiness-api-openapi.yml
- filename: apiosk-com-sources-api-openapi.yml
  format: yaml
  label: Apiosk Sources API
  slug: apiosk-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-sources-api-openapi.yml
- filename: apiosk-com-usage-api-openapi.yml
  format: yaml
  label: Apiosk Usage API
  slug: apiosk-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-usage-api-openapi.yml
auth_types: []
description: Apiosk uses organisation API keys presented as Bearer tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apiosk Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apiosk declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Apiosk
provider_slug: apiosk-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer apk_org_live_…'
  header: Authorization
  how_to_obtain: Create a key in the app under **Organisation → API keys**; the secret is shown once after creation.
  location: header
  name: Organisation API key
  scopes:
  - sources:read
  - sources:execute
  - ask:create
  - ask:execute
  - billing:read
  type: http-bearer
slug: apiosk-com-authentication
source_filename: apiosk-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.apiosk.com/api/authentication.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.apiosk.com/api/authentication.md\nsources:\n- https://docs.apiosk.com/api/authentication.md\n- https://docs.apiosk.com/app/api-keys.md\n- https://docs.apiosk.com/overview/quickstart.md\ndescription: Apiosk uses organisation API keys presented as Bearer tokens.\nschemes:\n- type: http-bearer\n  name: Organisation API key\n  evidence: 'Authorization: Bearer apk_org_live_…'\n  location: header\n  header: Authorization\n  scopes:\n  - sources:read\n  - sources:execute\n  - ask:create\n  - ask:execute\n  - billing:read\n  how_to_obtain: Create a key in the app under **Organisation → API keys**; the secret is shown once after creation.\ndocs: https://docs.apiosk.com/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/apiosk-com/authentication/apiosk-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Compliance
- Verification
- Sanctions
- Monitoring
- Company
---
