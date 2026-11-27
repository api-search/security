---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pandev-metrics-com-openapi-generated.yml
  format: yaml
  label: PanDev Metrics API
  slug: pandev-metrics-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pandev-metrics-com/openapi/_ae-authored/pandev-metrics-com-openapi-generated.yml
auth_types: []
description: Authentication methods for PanDev Metrics GitHub integration
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: PanDev Metrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: PanDev Metrics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PanDev Metrics
provider_slug: pandev-metrics-com
scheme_count: 1
schemes:
- evidence: 'paste a fine-grained PAT with Contents: Read and Pull requests: Read and write instead of going through the App install.'
  header: Authorization
  how_to_obtain: Paste a fine‑grained PAT into the GitHub integration screen in PanDev Metrics.
  location: header
  name: Personal Access Token
  type: http-bearer
slug: pandev-metrics-com-authentication
source_filename: pandev-metrics-com-authentication.yml
source_heading: Authentication Profile
source_url: https://pandev-metrics.com/docs/setup/git-integrations/github
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pandev-metrics.com/docs/setup/git-integrations/github\nsources:\n- https://pandev-metrics.com/docs/setup/git-integrations/github\n- https://pandev-metrics.com/docs/setup/ide-plugins/jetbrains-plugin\n- https://pandev-metrics.com/docs/setup/ide-plugins/vsc-plugin\n- https://pandev-metrics.com/docs/saas-getting-started\ndescription: Authentication methods for PanDev Metrics GitHub integration\nschemes:\n- type: http-bearer\n  name: Personal Access Token\n  evidence: 'paste a fine-grained PAT with Contents: Read and Pull requests: Read and write instead of going through the App install.'\n  location: header\n  header: Authorization\n  how_to_obtain: Paste a fine‑grained PAT into the GitHub integration screen in PanDev Metrics.\ndocs: https://pandev-metrics.com/docs/setup/git-integrations/github\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/pandev-metrics-com/authentication/pandev-metrics-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Engineering
- Metrics
- Platform
- B2B
---
