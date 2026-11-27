---
anonymous_access: false
api_key_in: []
api_specs:
- filename: launchflag-dev-evaluation-api-openapi.yml
  format: yaml
  label: LaunchFlag Evaluation API
  slug: launchflag-dev-evaluation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launchflag-dev/openapi/launchflag-dev-evaluation-api-openapi.yml
- filename: launchflag-dev-management-api-openapi.yml
  format: yaml
  label: LaunchFlag Management API
  slug: launchflag-dev-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launchflag-dev/openapi/launchflag-dev-management-api-openapi.yml
- filename: launchflag-dev-meta-api-openapi.yml
  format: yaml
  label: LaunchFlag Meta API
  slug: launchflag-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launchflag-dev/openapi/launchflag-dev-meta-api-openapi.yml
auth_types: []
description: LaunchFlag authenticates API requests using a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LaunchFlag Authentication
name_suffix: Authentication
oauth_flows: []
overview: LaunchFlag declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LaunchFlag
provider_slug: launchflag-dev
scheme_count: 1
schemes:
- evidence: The token always goes in the Authorization header or an env var, never in the URL.
  header: Authorization
  how_to_obtain: Obtain an API token from the LaunchFlag dashboard.
  location: header
  name: Authorization
  type: http-bearer
slug: launchflag-dev-authentication
source_filename: launchflag-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://launchflag.dev/docs
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://launchflag.dev/docs\nsources:\n- https://launchflag.dev/docs\ndescription: LaunchFlag authenticates API requests using a bearer token.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: The token always goes in the Authorization header or an env var, never in the URL.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an API token from the LaunchFlag dashboard.\ndocs: https://launchflag.dev/docs\n"
source_yaml_url: https://artifacts.apis.io/launchflag-dev/authentication/launchflag-dev-authentication.yml
summary_line: 1 scheme
tags:
- Feature Flags
- Kill Switch
- Rollouts
- Targeting
- Audit Logs
- SDK
---
