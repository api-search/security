---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes published on AgentMesh documentation
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentmesh Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentMesh declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentMesh
provider_slug: agentmesh-ai
scheme_count: 1
schemes:
- evidence: Access token The node's JWT on the transport plane. An amt_ bearer token on the HTTP plane.
  header: Authorization
  location: header
  name: amt_ token
  type: http-bearer
slug: agentmesh-ai-authentication
source_filename: agentmesh-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://dev.agentmesh.ai/authentication.html
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dev.agentmesh.ai/authentication.html\nsources:\n- https://dev.agentmesh.ai/authentication.html\n- https://dev.agentmesh.ai/for-google-credential.html\n- https://dev.agentmesh.ai/for-microsoft-credential.html\n- https://dev.agentmesh.ai/getting-started.html\ndescription: Authentication schemes published on AgentMesh documentation\nschemes:\n- type: http-bearer\n  name: amt_ token\n  evidence: Access token The node's JWT on the transport plane. An amt_ bearer token on the HTTP plane.\n  location: header\n  header: Authorization\ndocs: https://dev.agentmesh.ai/authentication.html\n"
source_yaml_url: https://artifacts.apis.io/agentmesh-ai/authentication/agentmesh-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Agents
- Platform
- Orchestration
---
