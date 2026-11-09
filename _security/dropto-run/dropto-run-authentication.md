---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dropto-run-abuse-api-openapi.yml
  format: yaml
  label: Dropto Abuse API
  slug: dropto-run-abuse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-abuse-api-openapi.yml
- filename: dropto-run-account-api-openapi.yml
  format: yaml
  label: Dropto Account API
  slug: dropto-run-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-account-api-openapi.yml
- filename: dropto-run-announcements-api-openapi.yml
  format: yaml
  label: Dropto Announcements API
  slug: dropto-run-announcements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-announcements-api-openapi.yml
- filename: dropto-run-auth-api-openapi.yml
  format: yaml
  label: Dropto Auth API
  slug: dropto-run-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-auth-api-openapi.yml
- filename: dropto-run-billing-api-openapi.yml
  format: yaml
  label: Dropto Billing API
  slug: dropto-run-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-billing-api-openapi.yml
- filename: dropto-run-deploys-api-openapi.yml
  format: yaml
  label: Dropto Deploys API
  slug: dropto-run-deploys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-deploys-api-openapi.yml
- filename: dropto-run-health-api-openapi.yml
  format: yaml
  label: Dropto Health API
  slug: dropto-run-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-health-api-openapi.yml
- filename: dropto-run-plans-api-openapi.yml
  format: yaml
  label: Dropto Plans API
  slug: dropto-run-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-plans-api-openapi.yml
- filename: dropto-run-promotions-api-openapi.yml
  format: yaml
  label: Dropto Promotions API
  slug: dropto-run-promotions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-promotions-api-openapi.yml
- filename: dropto-run-site-folders-api-openapi.yml
  format: yaml
  label: Dropto Site folders API
  slug: dropto-run-site-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-site-folders-api-openapi.yml
- filename: dropto-run-sites-api-openapi.yml
  format: yaml
  label: Dropto Sites API
  slug: dropto-run-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-sites-api-openapi.yml
- filename: dropto-run-support-api-openapi.yml
  format: yaml
  label: Dropto Support API
  slug: dropto-run-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-support-api-openapi.yml
- filename: dropto-run-tokens-api-openapi.yml
  format: yaml
  label: Dropto Tokens API
  slug: dropto-run-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-tokens-api-openapi.yml
auth_types: []
description: Dropto uses personal access tokens presented as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dropto Run Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dropto declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dropto
provider_slug: dropto-run
scheme_count: 1
schemes:
- evidence: 'curl -H "Authorization: Bearer d2r_..." https://dropto.run/api/sites'
  header: Authorization
  how_to_obtain: Obtain a personal access token via the CLI (`drop2run login` or `drop2run login --device`), the MCP server login tool, or manually from the Dropto web UI under Account → Access tokens.
  location: header
  name: Bearer token
  type: http-bearer
slug: dropto-run-authentication
source_filename: dropto-run-authentication.yml
source_heading: Authentication Profile
source_url: https://dropto.run/docs/auth.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dropto.run/docs/auth.md\nsources:\n- https://dropto.run/docs/auth.md\n- https://dropto.run/blog/hide-api-key-static-site\n- https://dropto.run/docs/auth\n- https://dropto.run/docs/api/auth\ndescription: Dropto uses personal access tokens presented as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'curl -H \"Authorization: Bearer d2r_...\" https://dropto.run/api/sites'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a personal access token via the CLI (`drop2run login` or `drop2run login --device`), the MCP server login tool, or manually\n    from the Dropto web UI under Account → Access tokens.\ndocs: https://dropto.run/docs/auth.md\n"
source_yaml_url: https://artifacts.apis.io/dropto-run/authentication/dropto-run-authentication.yml
summary_line: 1 scheme
tags:
- Hosting
- Artificial Intelligence
- Static Sites
- Developer Tools
- Cloud
---
