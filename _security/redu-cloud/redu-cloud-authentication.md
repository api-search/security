---
anonymous_access: false
api_key_in: []
api_specs:
- filename: redu-cloud-openapi-generated.yml
  format: yaml
  label: redu.cloud API
  slug: redu-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redu-cloud/openapi/_ae-authored/redu-cloud-openapi-generated.yml
auth_types: []
description: Authenticate requests to the redu.cloud API using an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: redu.cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: redu.cloud declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: redu.cloud
provider_slug: redu-cloud
scheme_count: 1
schemes:
- evidence: Authenticate requests to the redu.cloud API using an API key.
  header: x-api-key
  how_to_obtain: Generate an API key in the Console at https://console.redu.cloud/category/user/api-keys and copy it immediately.
  location: header
  name: API Key
  type: apiKey
slug: redu-cloud-authentication
source_filename: redu-cloud-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.redu.cloud/API/authentication
source_yaml: "generated: '2026-11-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.redu.cloud/API/authentication\nsources:\n- https://docs.redu.cloud/API/authentication\n- https://docs.redu.cloud/API/api-keys\n- https://docs.redu.cloud/Guides/quickstart\ndescription: Authenticate requests to the redu.cloud API using an API key.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Authenticate requests to the redu.cloud API using an API key.\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate an API key in the Console at https://console.redu.cloud/category/user/api-keys and copy it immediately.\ndocs: https://docs.redu.cloud/API/authentication\n"
source_yaml_url: https://artifacts.apis.io/redu-cloud/authentication/redu-cloud-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- Agent
- Deployment
- Infrastructure
- AI
---
