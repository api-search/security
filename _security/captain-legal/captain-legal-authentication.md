---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Captain.Legal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Captain.Legal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Captain.Legal
provider_slug: captain-legal
scheme_count: 2
schemes:
- applies_to:
  - list_document_types
  - get_requirements
  - generate_document
  - purchase_document
  description: 'Authentication: none for catalogue and preview'
  name: none
  type: none
- applies_to:
  - get_document_status
  description: get_document_status "Checks payment and delivery state using the private status token returned by the purchase tool." Per the docs, "Never expose the status token unless the user explicitly asks for it."
  name: status-token
  type: bearer-token-in-arguments
slug: captain-legal-authentication
source_filename: captain-legal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://mcp.captain.legal/docs/en/developers/\ndocs: https://mcp.captain.legal/docs/en/developers/\nschemes:\n- name: none\n  type: none\n  description: \"Authentication: none for catalogue and preview\"\n  applies_to: [list_document_types, get_requirements, generate_document, purchase_document]\n- name: status-token\n  type: bearer-token-in-arguments\n  description: get_document_status \"Checks payment and delivery state using the private status token returned by the purchase tool.\" Per the docs, \"Never expose the status token unless the user explicitly asks for it.\"\n  applies_to: [get_document_status]\nnote: The MCP endpoint (https://mcp.captain.legal/connect/) uses Streamable HTTP with an MCP session identifier returned on initialize. No API key, OAuth or account is documented. Payment happens on a signed Captain.Legal payment page, and \"Preview and payment URLs are signed and expire.\"\n"
source_yaml_url: https://artifacts.apis.io/captain-legal/authentication/captain-legal-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Legal
- Legal Documents
- Contracts
- Templates
- Legal Tech
- MCP
- AI Assistant
---
