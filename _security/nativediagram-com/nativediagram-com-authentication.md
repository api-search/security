---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for NativeDiagram API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NativeDiagram Authentication
name_suffix: Authentication
oauth_flows: []
overview: NativeDiagram declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NativeDiagram
provider_slug: nativediagram-com
scheme_count: 1
schemes:
- evidence: 'Use NativeDiagram through the xAI API with a NativeDiagram API key . Pass it as Authorization: Bearer <key> to the MCP server.'
  header: Authorization
  how_to_obtain: Obtain a NativeDiagram API key from the NativeDiagram account dashboard.
  location: header
  name: NativeDiagram API key
  type: http-bearer
slug: nativediagram-com-authentication
source_filename: nativediagram-com-authentication.yml
source_heading: Authentication Profile
source_url: https://nativediagram.com/docs/connect/grok/?goal=diagram
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nativediagram.com/docs/connect/grok/?goal=diagram\nsources:\n- https://nativediagram.com/docs/connect/grok/?goal=diagram\n- https://nativediagram.com/docs/connect/grok/?goal=document&format=docx\n- https://nativediagram.com/docs/skill/update/?client=grok\n- https://nativediagram.com/docs/start/?goal=diagram\ndescription: Authentication for NativeDiagram API\nschemes:\n- type: http-bearer\n  name: NativeDiagram API key\n  evidence: 'Use NativeDiagram through the xAI API with a NativeDiagram API key . Pass it as Authorization: Bearer <key> to the MCP server.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a NativeDiagram API key from the NativeDiagram account dashboard.\ndocs: https://nativediagram.com/docs/connect/grok/?goal=diagram\n"
source_yaml_url: https://artifacts.apis.io/nativediagram-com/authentication/nativediagram-com-authentication.yml
summary_line: 1 scheme
tags:
- SmartArt
- AI Assistant
- Microsoft Office
---
