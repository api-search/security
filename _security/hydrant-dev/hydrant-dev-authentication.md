---
anonymous_access: false
api_key_in: []
auth_types: []
description: Hydrant agents authenticate using a custom OAuth2 flow called service_auth. The agent registers via POST https://hydrant.dev/api/agent-auth/identity, receives a claim_token, polls https://hydrant.dev/api/auth/oauth2/token with grant_type=urn:workos:agent-auth:grant-type:claim to obtain an access_token, then uses the token as a Bearer token in the Authorization header for calls to https://hydrant.dev/api/mcp.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hydrant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hydrant declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hydrant
provider_slug: hydrant-dev
scheme_count: 1
schemes:
- evidence: 'Hydrant offers one: `service_auth`. You name the email address of the person who will approve, and that person does the approving.'
  flows:
  - urn:workos:agent-auth:grant-type:claim
  how_to_obtain: POST https://hydrant.dev/api/agent-auth/identity with JSON {"type":"service_auth","login_hint":"person@example.com","client_name":"Example agent"} to receive a claim_token, then poll the token endpoint with grant_type=urn:workos:agent-auth:grant-type:claim&claim_token=<claim_token>.
  name: service_auth
  scopes:
  - workspace.read
  - workspace.write
  token_url: https://hydrant.dev/api/auth/oauth2/token
  type: oauth2
slug: hydrant-dev-authentication
source_filename: hydrant-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://hydrant.dev/help/agents/auth-md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hydrant.dev/help/agents/auth-md\nsources:\n- https://hydrant.dev/help/agents/auth-md\n- https://hydrant.dev/auth.md\n- https://hydrant.dev/help/using/getting-started\ndescription: Hydrant agents authenticate using a custom OAuth2 flow called service_auth. The agent registers via POST https://hydrant.dev/api/agent-auth/identity,\n  receives a claim_token, polls https://hydrant.dev/api/auth/oauth2/token with grant_type=urn:workos:agent-auth:grant-type:claim to obtain an\n  access_token, then uses the token as a Bearer token in the Authorization header for calls to https://hydrant.dev/api/mcp.\nschemes:\n- type: oauth2\n  name: service_auth\n  evidence: 'Hydrant offers one: `service_auth`. You name the email address of the person who will approve, and that person does the approving.'\n  flows:\n  - urn:workos:agent-auth:grant-type:claim\n  token_url: https://hydrant.dev/api/auth/oauth2/token\n\
  \  scopes:\n  - workspace.read\n  - workspace.write\n  how_to_obtain: POST https://hydrant.dev/api/agent-auth/identity with JSON {\"type\":\"service_auth\",\"login_hint\":\"person@example.com\",\"client_name\":\"Example\n    agent\"} to receive a claim_token, then poll the token endpoint with grant_type=urn:workos:agent-auth:grant-type:claim&claim_token=<claim_token>.\ndocs: https://hydrant.dev/help/agents/auth-md\n"
source_yaml_url: https://artifacts.apis.io/hydrant-dev/authentication/hydrant-dev-authentication.yml
summary_line: 1 scheme
tags:
- Collaboration
- Project Management
- Artificial Intelligence
- Issue Tracking
- Software-as-a-Service
---
