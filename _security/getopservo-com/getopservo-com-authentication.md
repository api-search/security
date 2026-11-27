---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getopservo-com-openapi-generated.yml
  format: yaml
  label: Opservo API
  slug: getopservo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getopservo-com/openapi/_ae-authored/getopservo-com-openapi-generated.yml
auth_types: []
description: Authentication for Opservo API uses workspace API tokens sent in HTTP headers.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Opservo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opservo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Opservo
provider_slug: getopservo-com
scheme_count: 1
schemes:
- evidence: 'Either header works: Authorization: Bearer opv_…'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
slug: getopservo-com-authentication
source_filename: getopservo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getopservo.com/docs/agent-updates
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getopservo.com/docs/agent-updates\nsources:\n- https://getopservo.com/docs/agent-updates\n- https://getopservo.com/docs/api-tokens\n- https://staging.getopservo.com/changelog/2026-10-16-api-tokens-with-scopes-and-expiry-stronger-agent-signing\n- https://staging.getopservo.com/docs/api-tokens\ndescription: Authentication for Opservo API uses workspace API tokens sent in HTTP headers.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Either header works: Authorization: Bearer opv_…'\n  location: header\n  header: Authorization\nnote: No OAuth2 flows, API keys, or other authentication mechanisms are documented on the provided pages. 1 extracted row(s) were dropped because\n  their quote was not on the page.\ndocs: https://getopservo.com/docs/agent-updates\n"
source_yaml_url: https://artifacts.apis.io/getopservo-com/authentication/getopservo-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Linux
- Monitoring
- Automation
- Company
---
