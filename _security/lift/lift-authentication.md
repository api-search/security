---
api_key_in: []
auth_types:
- none
- bearer
description: ''
kind: authentication
layout: security
method: searched
name: Lift Authentication
name_suffix: Authentication
oauth_flows: []
overview: LIFT Aircraft secures its APIs with none and bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LIFT Aircraft
provider_slug: lift
scheme_count: 2
schemes:
- applies_to: https://www.liftaircraft.com/_api/mcp
  description: No authentication is required to connect to the MCP endpoint or to call read-only tools. Only public information published on the site is accessible.
  name: anonymous
  sources:
  - llms/lift-llms.txt
  type: none
- applies_to: CallWixSiteAPI
  description: A visitor access token obtained from the GenerateVisitorToken tool. Must be issued into the session before any CallWixSiteAPI request is made. Scoped to an anonymous visitor session, not to a user account.
  issued_by: GenerateVisitorToken
  name: visitorToken
  scheme: bearer
  sources:
  - llms/lift-llms.txt
  - mcp/lift-mcp.yml
  type: http
slug: lift-authentication
source_filename: lift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.liftaircraft.com/llms.txt\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nsummary:\n  types:\n  - none\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  note: LIFT Aircraft publishes no developer REST API and no OpenAPI. The only machine\n    surface is the Wix Site MCP endpoint, whose auth model is captured below.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: https://www.liftaircraft.com/_api/mcp\n  description: No authentication is required to connect to the MCP endpoint or to\n    call read-only tools. Only public information published on the site is accessible.\n  sources:\n  - llms/lift-llms.txt\n- name: visitorToken\n  type: http\n  scheme: bearer\n  applies_to: CallWixSiteAPI\n  description: A visitor access token obtained from the GenerateVisitorToken tool.\n    Must be issued into the session before any CallWixSiteAPI request is made. Scoped\n\
  \    to an anonymous visitor session, not to a user account.\n  issued_by: GenerateVisitorToken\n  sources:\n  - llms/lift-llms.txt\n  - mcp/lift-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lift/refs/heads/main/authentication/lift-authentication.yml
summary_line: none/bearer · 2 schemes
tags:
- Company
- Aviation
- eVTOL
- Electric Aircraft
- Urban Air Mobility
- Aerospace
- Transportation
- Experiential Entertainment
- Booking
- Model Context Protocol
---
