---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Custodo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Custodo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Custodo
provider_slug: custodo-ai
scheme_count: 2
schemes:
- access_levels:
  - Everything you can do
  - Read only
  applies_to: https://api.custodo.ai/mcp
  description: '"The first time it connects, it opens Custodo''s own authorisation page (OAuth 2.1): you sign in with your usual Custodo account and choose two things" -- which organisations, and «Everything you can do» or «Read only». Access is revoked from «Integrations» → «OAuth clients».'
  name: Custodo OAuth 2.1 (MCP)
  observed: Anonymous MCP initialize returns 401 "Missing bearer token" (recorded in apis.yml).
  type: oauth2
- description: '"One key, one address, and every function of Custodo is available to your line-of-business system or your script." A key never exceeds the person who created it and can be narrowed to certain modules, a ceiling per minute and per day, allowed source addresses, and destructive actions off until turned on.'
  name: API key
  source: https://custodo.ai/en/modules/
  type: apiKey
slug: custodo-ai-authentication
source_filename: custodo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://custodo.ai/llms.txt\ndocs: https://custodo.ai/en/ai-assistants/\nnote: No OpenAPI is published; schemes read from Custodo's own AI-assistant guide and Integrations module page (https://custodo.ai/en/modules/). The API reference itself is not public.\nschemes:\n- name: Custodo OAuth 2.1 (MCP)\n  type: oauth2\n  applies_to: https://api.custodo.ai/mcp\n  description: >-\n    \"The first time it connects, it opens Custodo's own authorisation page (OAuth 2.1): you sign in with your usual\n    Custodo account and choose two things\" -- which organisations, and «Everything you can do» or «Read only».\n    Access is revoked from «Integrations» → «OAuth clients».\n  access_levels:\n  - Everything you can do\n  - Read only\n  observed: Anonymous MCP initialize returns 401 \"Missing bearer token\" (recorded in apis.yml).\n- name: API key\n  type: apiKey\n  description: >-\n    \"One key, one address, and every function of Custodo\
  \ is available to your line-of-business system or your script.\" A key never exceeds the person who created it and can be narrowed to certain modules, a ceiling per minute and per day, allowed source addresses, and destructive actions off until turned on.\n  source: https://custodo.ai/en/modules/\n"
source_yaml_url: https://artifacts.apis.io/custodo-ai/authentication/custodo-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Document Management
- Business Management
- Small Business
- Digital Preservation
- E-Signature
- CRM
- Expense Management
- Time and Attendance
- AI Assistant
- MCP
- Italy
---
