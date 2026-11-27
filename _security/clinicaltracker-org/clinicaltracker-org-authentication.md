---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ClinicalTracker.org Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClinicalTracker.org declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ClinicalTracker.org
provider_slug: clinicaltracker-org
scheme_count: 3
schemes:
- applies_to: https://clinicaltracker.org/mcp
  evidence: Add it as a custom connector in your assistant. It asks you to sign in to clinicaltracker.org the first time, so there is no key to copy.
  name: mcp-connector-sign-in
  note: Sign-in flow type inferred as OAuth from the MCP connector pattern; the endpoint returns 401 anonymously (pre-flight dossier). Flow details and scopes are not documented.
  type: oauth2
- applies_to: https://clinicaltracker.org/api/clinical/v1
  evidence: Create a REST API key
  name: rest-api-key
  note: The homepage offers a "Create a REST API key" action; header name and format are not documented.
  type: apiKey
- applies_to: https://clinicaltracker.org/mcp/public
  evidence: No sign-in? Search-only connector https://clinicaltracker.org/mcp/public
  name: public-search-connector
  type: none
slug: clinicaltracker-org-authentication
source_filename: clinicaltracker-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clinicaltracker.org/\ndocs: https://clinicaltracker.org/docs/authentication\nschemes:\n- name: mcp-connector-sign-in\n  type: oauth2\n  applies_to: https://clinicaltracker.org/mcp\n  evidence: \"Add it as a custom connector in your assistant. It asks you to sign in to clinicaltracker.org the first time, so there is no key to copy.\"\n  note: Sign-in flow type inferred as OAuth from the MCP connector pattern; the endpoint returns 401 anonymously (pre-flight dossier). Flow details and scopes are not documented.\n- name: rest-api-key\n  type: apiKey\n  applies_to: https://clinicaltracker.org/api/clinical/v1\n  evidence: \"Create a REST API key\"\n  note: The homepage offers a \"Create a REST API key\" action; header name and format are not documented.\n- name: public-search-connector\n  type: none\n  applies_to: https://clinicaltracker.org/mcp/public\n  evidence: \"No sign-in? Search-only connector https://clinicaltracker.org/mcp/public\"\
  \nend_user_sign_in:\n- Email (no password, magic link for managing alerts)\n- Google (\"With Google, Google tells us your email address and confirms it is verified\")\nnote: The parent AgentStructure /docs/authentication page is a placeholder (\"AgentStructure does not currently issue API keys, OAuth clients, or access tokens from this website\"), so it contradicts the ClinicalTracker homepage and does not describe this product.\n"
source_yaml_url: https://artifacts.apis.io/clinicaltracker-org/authentication/clinicaltracker-org-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Clinical Trials
- Healthcare
- Life Sciences
- FDA
- Monitoring
- Alerts
- MCP
- AI Assistant
- Open Data
---
