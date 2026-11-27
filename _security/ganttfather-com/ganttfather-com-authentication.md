---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ganttfather-com-openapi-generated.yml
  format: yaml
  label: GanttFather API
  slug: ganttfather-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ganttfather-com/openapi/_ae-authored/ganttfather-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for GanttFather API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GanttFather Authentication
name_suffix: Authentication
oauth_flows: []
overview: GanttFather declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GanttFather
provider_slug: ganttfather-com
scheme_count: 1
schemes:
- evidence: "Every request carries your token as a Bearer header: \n Authorization: Bearer glt_YOUR_TOKEN"
  header: Authorization
  how_to_obtain: Create a token in the GanttFather app Settings → AI Agents & API and copy the glt_… value.
  location: header
  name: Bearer
  scopes:
  - Reads
  - Writes
  - Project token the granted project set
  - Account token any project you’re a member of (or own) — pass projectId explicitly
  type: http-bearer
slug: ganttfather-com-authentication
source_filename: ganttfather-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ganttfather.com/docs/api/authentication/
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ganttfather.com/docs/api/authentication/\nsources:\n- https://ganttfather.com/docs/api/authentication/\n- https://ganttfather.com/docs/api/introduction/\n- https://ganttfather.com/docs/api/list-projects/\n- https://ganttfather.com/article/monday-gantt-chart-guide/index.md\ndescription: Authentication schemes for GanttFather API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: \"Every request carries your token as a Bearer header: \\n Authorization: Bearer glt_YOUR_TOKEN\"\n  location: header\n  header: Authorization\n  scopes:\n  - Reads\n  - Writes\n  - Project token the granted project set\n  - Account token any project you’re a member of (or own) — pass projectId explicitly\n  how_to_obtain: Create a token in the GanttFather app Settings → AI Agents & API and copy the glt_… value.\nnote: No OAuth2, API key, or other authentication methods are documented.\n\
  docs: https://ganttfather.com/docs/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/ganttfather-com/authentication/ganttfather-com-authentication.yml
summary_line: 1 scheme
tags:
- Gantt Chart
- Project Management
- Collaboration
- Templates
- AI Assistant
- FreeSoftware
---
