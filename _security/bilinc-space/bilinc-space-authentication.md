---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bilinc-space-openapi-generated.yml
  format: yaml
  label: Bilinc API
  slug: bilinc-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bilinc-space/openapi/_ae-authored/bilinc-space-openapi-generated.yml
auth_types: []
description: Bilinc uses an API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bilinc Space Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bilinc declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bilinc
provider_slug: bilinc-space
scheme_count: 1
schemes:
- evidence: Use the API key only as a bearer token. Never print, log, commit, or expose it.
  header: Authorization
  how_to_obtain: Create a Cloud key from the dashboard or via `bilinc login` which saves the key locally; the key can also be set in the environment variable BILINC_API_KEY.
  location: header
  name: Bearer
  type: http-bearer
slug: bilinc-space-authentication
source_filename: bilinc-space-authentication.yml
source_heading: Authentication Profile
source_url: https://bilinc.space/docs/quickstart
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bilinc.space/docs/quickstart\nsources:\n- https://bilinc.space/docs/quickstart\n- https://bilinc.space/docs/cloud-quickstart\ndescription: Bilinc uses an API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Use the API key only as a bearer token. Never print, log, commit, or expose it.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Cloud key from the dashboard or via `bilinc login` which saves the key locally; the key can also be set in the environment\n    variable BILINC_API_KEY.\ndocs: https://bilinc.space/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/bilinc-space/authentication/bilinc-space-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Platform
- Developer Tools
- Cloud
---
