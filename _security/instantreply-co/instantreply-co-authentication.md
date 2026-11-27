---
anonymous_access: false
api_key_in: []
api_specs:
- filename: instantreply-co-openapi-generated.yml
  format: yaml
  label: Instant Reply API
  slug: instantreply-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instantreply-co/openapi/_ae-authored/instantreply-co-openapi-generated.yml
auth_types: []
description: Authentication uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Instant Reply Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instant Reply declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Instant Reply
provider_slug: instantreply-co
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer $IR_API_KEY"'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys, then copy the key.
  location: header
  name: Bearer
  type: http-bearer
slug: instantreply-co-authentication
source_filename: instantreply-co-authentication.yml
source_heading: Authentication Profile
source_url: https://www.instantreply.co/ar/developers/quickstart
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.instantreply.co/ar/developers/quickstart\nsources:\n- https://www.instantreply.co/ar/developers/quickstart\n- https://www.instantreply.co/developers/quickstart\n- https://www.instantreply.co/agents\n- https://www.instantreply.co/es/developers/quickstart\ndescription: Authentication uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '-H \"Authorization: Bearer $IR_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys, then copy the key.\ndocs: https://www.instantreply.co/ar/developers/quickstart\n"
source_yaml_url: https://artifacts.apis.io/instantreply-co/authentication/instantreply-co-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Chatbots
- Social Messaging
- Lead Generation
- Automation
---
