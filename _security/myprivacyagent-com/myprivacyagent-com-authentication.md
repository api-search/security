---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for My Privacy Agent MCP connector
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: My Privacy Agent Authentication
name_suffix: Authentication
oauth_flows: []
overview: My Privacy Agent declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: My Privacy Agent
provider_slug: myprivacyagent-com
scheme_count: 1
schemes:
- evidence: 'Six account tools are available after OAuth sign-in: list_my_subjects, get_my_report, list_my_cases, get_case_status, request_recheck, and submit_approved_plan.'
  how_to_obtain: Tokens must come from Clerk for this exact MCP endpoint; tokens for another resource are rejected.
  name: OAuth2
  type: oauth2
slug: myprivacyagent-com-authentication
source_filename: myprivacyagent-com-authentication.yml
source_heading: Authentication Profile
source_url: https://myprivacyagent.com/docs/mcp-account.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://myprivacyagent.com/docs/mcp-account.md\nsources:\n- https://myprivacyagent.com/docs/mcp-account.md\ndescription: Authentication for My Privacy Agent MCP connector\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: 'Six account tools are available after OAuth sign-in: list_my_subjects, get_my_report, list_my_cases, get_case_status, request_recheck,\n    and submit_approved_plan.'\n  how_to_obtain: Tokens must come from Clerk for this exact MCP endpoint; tokens for another resource are rejected.\ndocs: https://myprivacyagent.com/docs/mcp-account.md\n"
source_yaml_url: https://artifacts.apis.io/myprivacyagent-com/authentication/myprivacyagent-com-authentication.yml
summary_line: 1 scheme
tags:
- Personal Information Removal
- Data Broker Opt‑out
---
