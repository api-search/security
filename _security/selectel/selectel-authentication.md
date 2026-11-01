---
anonymous_access: false
api_key_in: []
api_specs:
- filename: selectel-openapi-generated.yml
  format: yaml
  label: Selectel API
  slug: selectel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/selectel/openapi/_ae-authored/selectel-openapi-generated.yml
auth_types: []
description: Selectel authentication uses tokens passed in HTTP headers.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Selectel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Selectel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Selectel
provider_slug: selectel
scheme_count: 1
schemes:
- evidence: 'IAM tokens are passed in the X-Auth-Token header and have different scopes:'
  header: X-Auth-Token
  how_to_obtain: Obtain an account‑scoped or project‑scoped IAM token via the OpenStack identity API (POST to https://cloud.api.selcloud.ru/identity/v3/auth/tokens).
  location: header
  name: X-Auth-Token
  type: apiKey
slug: selectel-authentication
source_filename: selectel-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.selectel.ru/en/api/authorization/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.selectel.ru/en/api/authorization/\nsources:\n- https://docs.selectel.ru/en/api/authorization/\n- https://docs.selectel.ru/en/api/craas/\ndescription: Selectel authentication uses tokens passed in HTTP headers.\nschemes:\n- type: apiKey\n  name: X-Auth-Token\n  evidence: 'IAM tokens are passed in the X-Auth-Token header and have different scopes:'\n  location: header\n  header: X-Auth-Token\n  how_to_obtain: Obtain an account‑scoped or project‑scoped IAM token via the OpenStack identity API (POST to https://cloud.api.selcloud.ru/identity/v3/auth/tokens).\ndocs: https://docs.selectel.ru/en/api/authorization/\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/selectel/authentication/selectel-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- Infrastructure
- VPS
- Storage
- Kubernetes
---
