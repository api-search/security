---
anonymous_access: false
api_key_in: []
api_specs:
- filename: calluponit-com-openapi-generated.yml
  format: yaml
  label: CallUpOnIt API
  slug: calluponit-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calluponit-com/openapi/_ae-authored/calluponit-com-openapi-generated.yml
auth_types: []
description: Authentication schemes as published on the CallUpOnIt Agent API page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Calluponit Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CallUpOnIt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CallUpOnIt
provider_slug: calluponit-com
scheme_count: 1
schemes:
- evidence: 'Send Authorization: Bearer YOUR_AGENT_KEY.'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: calluponit-com-authentication
source_filename: calluponit-com-authentication.yml
source_heading: Authentication Profile
source_url: https://calluponit.com/agent-api
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://calluponit.com/agent-api\nsources:\n- https://calluponit.com/agent-api\ndescription: Authentication schemes as published on the CallUpOnIt Agent API page.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send Authorization: Bearer YOUR_AGENT_KEY.'\n  location: header\n  header: Authorization\ndocs: https://calluponit.com/agent-api\n"
source_yaml_url: https://artifacts.apis.io/calluponit-com/authentication/calluponit-com-authentication.yml
summary_line: 1 scheme
tags:
- Reminders
- voice-calls
- Email Scheduling
- AI Agents
---
