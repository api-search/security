---
anonymous_access: false
api_key_in: []
auth_types: []
description: Agent Community uses a custom OAuth2 flow called `service_auth`.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentcommunity Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Community declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Community
provider_slug: agentcommunity-org
scheme_count: 1
schemes:
- evidence: 'Send the access token only in the Authorization header:'
  how_to_obtain: Register via POST /agent/identity to receive a claim token, then poll POST /oauth2/token with grant_type=urn:workos:agent-auth:grant-type:claim and the claim_token; alternatively exchange the service‑signed JWT using grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer.
  name: service_auth
  scopes:
  - agent.account.read
  - agent.registrations.read
  token_url: /oauth2/token
  type: oauth2
slug: agentcommunity-org-authentication
source_filename: agentcommunity-org-authentication.yml
source_heading: Authentication Profile
source_url: https://agentcommunity.org/auth.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentcommunity.org/auth.md\nsources:\n- https://agentcommunity.org/auth.md\n- https://agentcommunity.org/blog/web_auth_box_not_for_agents.md\n- https://agentcommunity.org/blog/aid-auth-md-alignment.md\n- https://agentcommunity.org/docs/agent-onboarding.md\ndescription: Agent Community uses a custom OAuth2 flow called `service_auth`.\nschemes:\n- type: oauth2\n  name: service_auth\n  evidence: 'Send the access token only in the Authorization header:'\n  token_url: /oauth2/token\n  scopes:\n  - agent.account.read\n  - agent.registrations.read\n  how_to_obtain: Register via POST /agent/identity to receive a claim token, then poll POST /oauth2/token with grant_type=urn:workos:agent-auth:grant-type:claim\n    and the claim_token; alternatively exchange the service‑signed JWT using grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer.\ndocs: https://agentcommunity.org/auth.md\n"
source_yaml_url: https://artifacts.apis.io/agentcommunity-org/authentication/agentcommunity-org-authentication.yml
summary_line: 1 scheme
tags:
- Community
- Open Source
- Agents
- Governance
- Collaboration
---
