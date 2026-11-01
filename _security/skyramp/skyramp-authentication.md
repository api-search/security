---
anonymous_access: false
api_key_in: []
api_specs:
- filename: skyramp-openapi-generated.yml
  format: yaml
  label: Skyramp API
  slug: skyramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skyramp/openapi/_ae-authored/skyramp-openapi-generated.yml
auth_types: []
description: Skyramp tests expect a Bearer Token by default and also support additional authentication methods. The token is provided via the environment variable `SKYRAMP_TEST_TOKEN` and is sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Skyramp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skyramp declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Skyramp
provider_slug: skyramp
scheme_count: 1
schemes:
- evidence: By default, Skyramp expects a Bearer Token but we support additional authentication methods (Example 3).
  header: Authorization
  how_to_obtain: Set the environment variable `SKYRAMP_TEST_TOKEN` to your authentication token (e.g., session_id obtained from the Demo Shop UI).
  location: header
  name: Bearer Token
  type: http-bearer
slug: skyramp-authentication
source_filename: skyramp-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.skyramp.dev/quickstart/first-test
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.skyramp.dev/quickstart/first-test\nsources:\n- https://docs.skyramp.dev/quickstart/first-test\n- https://docs.skyramp.dev/quickstart/install\n- https://docs.skyramp.dev/\ndescription: Skyramp tests expect a Bearer Token by default and also support additional authentication methods. The token is provided via the\n  environment variable `SKYRAMP_TEST_TOKEN` and is sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: By default, Skyramp expects a Bearer Token but we support additional authentication methods (Example 3).\n  location: header\n  header: Authorization\n  how_to_obtain: Set the environment variable `SKYRAMP_TEST_TOKEN` to your authentication token (e.g., session_id obtained from the Demo Shop\n    UI).\ndocs: https://docs.skyramp.dev/quickstart/first-test\n"
source_yaml_url: https://artifacts.apis.io/skyramp/authentication/skyramp-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Testing
- DeveloperTools
- Automation
---
