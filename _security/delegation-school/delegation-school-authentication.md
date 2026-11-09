---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: none
name: Delegation School Authentication
name_suffix: Authentication
oauth_flows: []
overview: delegation.school declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: delegation.school
provider_slug: delegation-school
scheme_count: 0
schemes: []
slug: delegation-school-authentication
source_filename: delegation-school-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: 'name: delegation.school authentication

  generated: ''2026-11-05''

  method: none

  source: https://delegation.school/connect/

  docs: https://delegation.school/help/

  schemes: []

  anonymous: true

  summary: The remote MCP server at https://delegation.school/mcp requires no credentials. The Connect page states "No login or API key — it''s open and read-only."

  notes:

  - ''The Help page says Claude''''s "Add custom connector" step may try to set up a sign-in anyway and fail with "Couldn''''t register with delegation.school''''s sign-in service"; the documented fix is to paste only the URL and leave any "Advanced" / "OAuth Client ID" section blank. There is no OAuth flow to register with.''

  - Learner progress is keyed to the email the learner gives the tutor ("Your progress now follows your email, not your name", changelog June 8, 2026); this is an identifier, not an authentication scheme.

  '
source_yaml_url: https://artifacts.apis.io/delegation-school/authentication/delegation-school-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Artificial Intelligence
- Education
- Online Courses
- MCP
- AI Agents
- Productivity
---
