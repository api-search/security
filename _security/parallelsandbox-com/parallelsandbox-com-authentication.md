---
anonymous_access: false
api_key_in: []
api_specs:
- filename: parallelsandbox-com-openapi-generated.yml
  format: yaml
  label: ParallelSandbox API
  slug: parallelsandbox-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parallelsandbox-com/openapi/_ae-authored/parallelsandbox-com-openapi-generated.yml
auth_types: []
description: Authentication methods for ParallelSandbox
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ParallelSandbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: ParallelSandbox declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ParallelSandbox
provider_slug: parallelsandbox-com
scheme_count: 2
schemes:
- evidence: Each teammate, or each agent, connects with the one line from Quick start and signs in to the account in the browser once (OAuth).
  name: OAuth
  type: oauth2
- evidence: 'Only tools without OAuth need a psbx_ API key: the account owner makes one per teammate or agent over REST with the app''s signed-in session ( POST /v1/keys with a name; shown once).'
  how_to_obtain: Create via POST /v1/keys in the signed‑in app session
  name: psbx_ API key
  type: apiKey
slug: parallelsandbox-com-authentication
source_filename: parallelsandbox-com-authentication.yml
source_heading: Authentication Profile
source_url: https://parallelsandbox.com/en/docs/quickstart/
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://parallelsandbox.com/en/docs/quickstart/\nsources:\n- https://parallelsandbox.com/en/docs/quickstart/\n- https://parallelsandbox.com/en/docs/team-setup/\n- https://parallelsandbox.com/en/docs/quickstart\n- https://parallelsandbox.com/en/docs/team-setup\ndescription: Authentication methods for ParallelSandbox\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Each teammate, or each agent, connects with the one line from Quick start and signs in to the account in the browser once (OAuth).\n- type: apiKey\n  name: psbx_ API key\n  evidence: 'Only tools without OAuth need a psbx_ API key: the account owner makes one per teammate or agent over REST with the app''s signed-in\n    session ( POST /v1/keys with a name; shown once).'\n  how_to_obtain: Create via POST /v1/keys in the signed‑in app session\ndocs: https://parallelsandbox.com/en/docs/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/parallelsandbox-com/authentication/parallelsandbox-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Sandbox
- Testing
- UX
- Developer Tools
---
