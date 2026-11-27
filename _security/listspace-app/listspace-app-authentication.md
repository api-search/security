---
anonymous_access: false
api_key_in: []
api_specs:
- filename: listspace-app-openapi-generated.yml
  format: yaml
  label: Listspace API
  slug: listspace-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listspace-app/openapi/_ae-authored/listspace-app-openapi-generated.yml
auth_types: []
description: Authentication methods for Listspace as described on the documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Listspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Listspace declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Listspace
provider_slug: listspace-app
scheme_count: 2
schemes:
- evidence: Sign-in (OAuth) means your AI sends you to Listspace, where you sign in with your Listspace account and click Allow.
  how_to_obtain: User is redirected to Listspace to sign in and authorize the application.
  name: Listspace OAuth
  type: oauth2
- evidence: In Claude, choose No sign-in under Authentication, and under Request headers add the name Authorization with the value Bearer , a space, then your token.
  header: Authorization
  how_to_obtain: Create a token in Settings > Your AI > API tokens and copy it.
  location: header
  name: Listspace Token
  type: apiKey
slug: listspace-app-authentication
source_filename: listspace-app-authentication.yml
source_heading: Authentication Profile
source_url: https://listspace.app/docs/mcp
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://listspace.app/docs/mcp\nsources:\n- https://listspace.app/docs/mcp\n- https://listspace.app/setup\ndescription: Authentication methods for Listspace as described on the documentation pages.\nschemes:\n- type: oauth2\n  name: Listspace OAuth\n  evidence: Sign-in (OAuth) means your AI sends you to Listspace, where you sign in with your Listspace account and click Allow.\n  how_to_obtain: User is redirected to Listspace to sign in and authorize the application.\n- type: apiKey\n  name: Listspace Token\n  evidence: In Claude, choose No sign-in under Authentication, and under Request headers add the name Authorization with the value Bearer , a\n    space, then your token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in Settings > Your AI > API tokens and copy it.\ndocs: https://listspace.app/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/listspace-app/authentication/listspace-app-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Collaboration
- Memory
- Agents
- Platform
---
