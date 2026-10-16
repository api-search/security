---
anonymous_access: false
api_key_in: []
api_specs:
- filename: machinemetrics-openapi-generated.yml
  format: yaml
  label: MachineMetrics API
  slug: machinemetrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinemetrics/refs/heads/main/openapi/_ae-authored/machinemetrics-openapi-generated.yml
auth_types: []
description: Authentication with API keys using Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Machinemetrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: MachineMetrics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MachineMetrics
provider_slug: machinemetrics
scheme_count: 1
schemes:
- evidence: In both cases, our system leverages Bearer tokens in the Authorization header as a means to authenticate.
  header: Authorization
  how_to_obtain: Navigate to https://app.machinemetrics.com/app/settings/api-keys and create an API Key.
  location: header
  name: Bearer
  type: http-bearer
slug: machinemetrics-authentication
source_filename: machinemetrics-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.machinemetrics.com/docs/data-and-apis/authentication/
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.machinemetrics.com/docs/data-and-apis/authentication/\nsources:\n- https://developers.machinemetrics.com/docs/data-and-apis/authentication/\n- https://developers.machinemetrics.com/docs/build-apps/authentication/\n- https://developers.machinemetrics.com/docs/tools/mmdev-cli/authentication/\n- https://developers.machinemetrics.com/docs/tools/mmdev-cli/oauth-management/\ndescription: Authentication with API keys using Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: In both cases, our system leverages Bearer tokens in the Authorization header as a means to authenticate.\n  location: header\n  header: Authorization\n  how_to_obtain: Navigate to https://app.machinemetrics.com/app/settings/api-keys and create an API Key.\nnote: No OAuth flows or additional authentication schemes are documented on the provided pages.\n\
  docs: https://developers.machinemetrics.com/docs/data-and-apis/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinemetrics/refs/heads/main/authentication/machinemetrics-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Manufacturing
- AI
- MES
- IoT
- SaaS
---
