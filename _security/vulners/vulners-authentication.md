---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vulners-openapi-generated.yml
  format: yaml
  label: Vulners API
  slug: vulners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulners/openapi/_ae-authored/vulners-openapi-generated.yml
auth_types: []
description: Authentication methods for Vulners API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vulners Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vulners declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vulners
provider_slug: vulners
scheme_count: 1
schemes:
- evidence: Vulners API uses API keys via HTTP headers for all authenticated requests.
  header: X-Api-Key
  how_to_obtain: Register an account, log in, go to the API keys tab, generate an API key, and save it.
  location: header
  name: X-Api-Key
  type: apiKey
slug: vulners-authentication
source_filename: vulners-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.vulners.com/docs/quickstart/authentication/
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.vulners.com/docs/quickstart/authentication/\nsources:\n- https://docs.vulners.com/docs/quickstart/authentication/\n- https://docs.vulners.com/docs/quickstart/api_key/\n- https://docs.vulners.com/docs/quickstart/authentication/\n- https://docs.vulners.com/docs/quickstart/\ndescription: Authentication methods for Vulners API\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: Vulners API uses API keys via HTTP headers for all authenticated requests.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Register an account, log in, go to the API keys tab, generate an API key, and save it.\ndocs: https://docs.vulners.com/docs/quickstart/authentication/\n"
source_yaml_url: https://artifacts.apis.io/vulners/authentication/vulners-authentication.yml
summary_line: 1 scheme
tags:
- Security
- Vulnerabilities
- Intelligence
- Platform
---
