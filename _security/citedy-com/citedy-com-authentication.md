---
anonymous_access: false
api_key_in: []
auth_types: []
description: Client authenticates using a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Citedy Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Citedy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Citedy
provider_slug: citedy-com
scheme_count: 1
schemes:
- evidence: Authorization string header required Bearer citedy_agent_* key
  header: Authorization
  how_to_obtain: Register the agent via the public registration endpoint, approve the request in the browser, and copy the API key that starts with citedy_agent_.
  location: header
  name: Bearer token
  type: http-bearer
slug: citedy-com-authentication
source_filename: citedy-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.citedy.com/docs/api-reference/agent/rotate-current-agent-api-key
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.citedy.com/docs/api-reference/agent/rotate-current-agent-api-key\nsources:\n- https://www.citedy.com/docs/api-reference/agent/rotate-current-agent-api-key\n- https://www.citedy.com/docs/quickstart\ndescription: Client authenticates using a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Authorization string header required Bearer citedy_agent_* key\n  location: header\n  header: Authorization\n  how_to_obtain: Register the agent via the public registration endpoint, approve the request in the browser, and copy the API key that starts\n    with citedy_agent_.\ndocs: https://www.citedy.com/docs/api-reference/agent/rotate-current-agent-api-key\n"
source_yaml_url: https://artifacts.apis.io/citedy-com/authentication/citedy-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- SEO
- Content Automation
- Agents
- Platform
---
