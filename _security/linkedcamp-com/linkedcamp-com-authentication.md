---
anonymous_access: false
api_key_in: []
api_specs:
- filename: linkedcamp-com-openapi-generated.yml
  format: yaml
  label: Linkedcamp API
  slug: linkedcamp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedcamp-com/openapi/_ae-authored/linkedcamp-com-openapi-generated.yml
auth_types: []
description: LinkedCamp uses a simple API token passed in a request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Linkedcamp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linkedcamp declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Linkedcamp
provider_slug: linkedcamp-com
scheme_count: 1
schemes:
- evidence: Every authenticated request must include a `token` header containing your API key.
  header: token
  how_to_obtain: From the Dashboard under Settings → API, or via the Get API Token endpoint for agency owners.
  location: header
  name: API Token
  type: apiKey
slug: linkedcamp-com-authentication
source_filename: linkedcamp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.linkedcamp.com/authentication.md
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.linkedcamp.com/authentication.md\nsources:\n- https://docs.linkedcamp.com/authentication.md\n- https://help.linkedcamp.com/en/articles/5975172-api-keys\n- https://docs.linkedcamp.com/api-reference/users/get-token.md\n- https://docs.linkedcamp.com/api-reference/tokens/get-api-token.md\ndescription: LinkedCamp uses a simple API token passed in a request header.\nschemes:\n- type: apiKey\n  name: API Token\n  evidence: Every authenticated request must include a `token` header containing your API key.\n  location: header\n  header: token\n  how_to_obtain: From the Dashboard under Settings → API, or via the Get API Token endpoint for agency owners.\ndocs: https://docs.linkedcamp.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/linkedcamp-com/authentication/linkedcamp-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Lead Generation
- Artificial Intelligence
- Automation
- LinkedIn
---
