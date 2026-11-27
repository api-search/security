---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: DIKOO Authentication
name_suffix: Authentication
oauth_flows: []
overview: DIKOO declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DIKOO
provider_slug: dikoo-fr
scheme_count: 1
schemes:
- applies_to: https://www.dikoo.fr/mcp
  evidence: 'Transport : HTTP streamable (Model Context Protocol), sans authentification, lecture seule.'
  name: none
  type: none
slug: dikoo-fr-authentication
source_filename: dikoo-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://www.dikoo.fr/ia\ndocs: https://www.dikoo.fr/llms-full.txt\nnote: 'The only public interface is the MCP server, documented as unauthenticated (\"Authentification : aucune\"; \"sans authentification, lecture seule\"). Other /api/* paths are documented as internal and were not called. No OpenAPI securitySchemes exist.'\nschemes:\n- name: none\n  type: none\n  applies_to: https://www.dikoo.fr/mcp\n  evidence: 'Transport : HTTP streamable (Model Context Protocol), sans authentification, lecture seule.'\n"
source_yaml_url: https://artifacts.apis.io/dikoo-fr/authentication/dikoo-fr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Legal
- Lawyers
- Legal Directory
- Appointment Booking
- Legal Tech
- MCP
- Artificial Intelligence
- France
---
