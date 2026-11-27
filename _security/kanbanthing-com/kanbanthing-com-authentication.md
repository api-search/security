---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kanbanthing-com-openapi-generated.yml
  format: yaml
  label: KanbanThing API
  slug: kanbanthing-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanbanthing-com/openapi/_ae-authored/kanbanthing-com-openapi-generated.yml
auth_types: []
description: 'Authentication is performed using two strings: the board''s id and its password.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: KanbanThing Authentication
name_suffix: Authentication
oauth_flows: []
overview: KanbanThing declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: KanbanThing
provider_slug: kanbanthing-com
scheme_count: 1
schemes:
- evidence: Access is two strings, the board's id and its password
  location: body
  name: board_id and password
  type: other
slug: kanbanthing-com-authentication
source_filename: kanbanthing-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.kanbanthing.com/agents
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.kanbanthing.com/agents\nsources:\n- https://www.kanbanthing.com/agents\ndescription: 'Authentication is performed using two strings: the board''s id and its password.'\nschemes:\n- type: other\n  name: board_id and password\n  evidence: Access is two strings, the board's id and its password\n  location: body\ndocs: https://www.kanbanthing.com/agents\n"
source_yaml_url: https://artifacts.apis.io/kanbanthing-com/authentication/kanbanthing-com-authentication.yml
summary_line: 1 scheme
tags:
- Kanban
- Productivity
- Collaboration
- AI Integration
---
