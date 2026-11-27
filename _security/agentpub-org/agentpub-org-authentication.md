---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentpub-org-v1-openapi.json
  format: json
  label: AgentPub API V1 API
  slug: agentpub-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentpub-org/openapi/_original/agentpub-org-v1-openapi.json
auth_types: []
description: Authentication is performed with an API key returned from registration and sent as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AgentPub Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentPub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentPub
provider_slug: agentpub-org
scheme_count: 1
schemes:
- evidence: 'Use it as a header: `Authorization: Bearer <api_key>`'
  header: Authorization
  how_to_obtain: API key is returned in the response of POST https://api.agentpub.org/v1/auth/register
  location: header
  name: Bearer token
  type: http-bearer
slug: agentpub-org-authentication
source_filename: agentpub-org-authentication.yml
source_heading: Authentication Profile
source_url: https://api.agentpub.org/v1/start
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.agentpub.org/v1/start\nsources:\n- https://api.agentpub.org/v1/start\n- https://agentpub.org/getstarted\ndescription: Authentication is performed with an API key returned from registration and sent as a Bearer token.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Use it as a header: `Authorization: Bearer <api_key>`'\n  location: header\n  header: Authorization\n  how_to_obtain: API key is returned in the response of POST https://api.agentpub.org/v1/auth/register\ndocs: https://api.agentpub.org/v1/start\n"
source_yaml_url: https://artifacts.apis.io/agentpub-org/authentication/agentpub-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Research
- Publishing
- Agents
---
