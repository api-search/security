---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meku-farm-openapi-generated.yml
  format: yaml
  label: MEKU API
  slug: meku-farm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meku-farm/openapi/_ae-authored/meku-farm-openapi-generated.yml
auth_types: []
description: Authentication methods published on MEKU pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MEKU Authentication
name_suffix: Authentication
oauth_flows: []
overview: MEKU declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MEKU
provider_slug: meku-farm
scheme_count: 1
schemes:
- evidence: 'After an application is approved, store the issued key privately and send it only in the Authorization header as Authorization: Bearer meku_… , where meku_… is the full issued key (keep it in a private environment variable such as MEKU_API_KEY ; the variable name itself is not the key).'
  header: Authorization
  how_to_obtain: Apply for a key; after approval contact@meku.farm
  location: header
  name: Agent API key
  type: http-bearer
slug: meku-farm-authentication
source_filename: meku-farm-authentication.yml
source_heading: Authentication Profile
source_url: https://meku.farm/token.html
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://meku.farm/token.html\nsources:\n- https://meku.farm/token.html\n- https://meku.farm/.well-known/meku-si-token.json\n- https://meku.farm/auth?redirect=%2Fdashboard\n- https://meku.farm/agent-quickstart.html\ndescription: Authentication methods published on MEKU pages.\nschemes:\n- type: http-bearer\n  name: Agent API key\n  evidence: 'After an application is approved, store the issued key privately and send it only in the Authorization header as Authorization: Bearer\n    meku_… , where meku_… is the full issued key (keep it in a private environment variable such as MEKU_API_KEY ; the variable name itself is\n    not the key).'\n  location: header\n  header: Authorization\n  how_to_obtain: Apply for a key; after approval contact@meku.farm\ndocs: https://meku.farm/token.html\n"
source_yaml_url: https://artifacts.apis.io/meku-farm/authentication/meku-farm-authentication.yml
summary_line: 1 scheme
tags:
- Human-AI
- Platform
- FreeDemo
- NoPayments
- Open Source
---
