---
anonymous_access: true
api_key_in: []
api_specs:
- filename: luthersystems-com-agentsearch-openapi.yml
  format: yaml
  label: AgentSearch HTTP API
  slug: agentsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luthersystems-com/refs/heads/main/openapi/luthersystems-com-agentsearch-openapi.yml
auth_types: []
description: 'Three distinct postures. AgentSearch is anonymous end to end — no keys, the card declares securitySchemes.public.type "none". InsideOut is anonymous for design and pricing but session-scoped: convoopen mints a session_id whose ?token= suffix is the per-session credential, deployment requires the user to connect AWS/GCP credentials in a browser (the cloud provider''s own OAuth, never passed through the agent) and to subscribe, and the A2A tasks/get method requires an X-A2A-Task-Secret header. The Luther Enterprise platform (customer-deployed) authenticates with RS256 JWTs issued by LutherAuth against external OIDC IdPs (Cognito, AzureAD, Auth0), with API-key pre-validation supported by the Go SDK and an X-API-KEY header on the starter-kit middleware API.'
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Luthersystems Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luther Systems declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Luther Systems
provider_slug: luthersystems-com
scheme_count: 6
schemes:
- api: AgentSearch (HTTP, MCP, A2A)
  description: All endpoints publicly readable; no credential of any kind. Rate limiting is per IP, best effort.
  evidence: agent card securitySchemes.public is {"type":"none"}; OpenAPI has no securitySchemes/security; MCP initialize + tools/list answered anonymously.
  name: public
  type: none
- api: InsideOut MCP (https://app.luthersystems.com/v1/insideout-mcp)
  description: convoopen returns session_id in the form sess_v2_xxx?token=yyy; the token is part of the session id and must be sent verbatim on every later tool call. No user-supplied API key. Mcp-Session-Id header carries the MCP transport session.
  evidence: convoopen tool description (live tools/list); SKILL.md "No API keys required from the user".
  name: insideout-session-token
  scopes: none
  type: bearer-in-session-id
- api: InsideOut MCP (tfdeploy, tfdestroy, awsinspect, gcpinspect)
  description: Deployment and inspection need the user to open a connect URL, authenticate directly with AWS or GCP and subscribe to a Luther Systems plan; credawait polls for completion. Credentials are held by the InsideOut platform, never by the agent or skill.
  evidence: credawait tool description; SECURITY.md "Cloud credentials" section.
  name: cloud-credential-connect
  type: delegated (browser-based cloud-provider OAuth, out of band)
- api: InsideOut A2A (https://insideout.luthersystems.com/insideout-a2a/v0/)
  description: Required by tasks/get; not declared in the card's securitySchemes.
  evidence: 'live -32602 "X-A2A-Task-Secret header is required: invalid params".'
  header: X-A2A-Task-Secret
  in: header
  name: x-a2a-task-secret
  type: apiKey
- api: Luther Enterprise platform (customer-deployed middleware / gRPC)
  bearer_format: JWT (RS256)
  description: Tokens issued by LutherAuth after OAuth/OIDC login with an external IdP; validated from gRPC metadata, HTTP cookies or headers via lutherauth-sdk-go with JWK caching and CSRF nonces. LutherAuth v4.7.6 added Auth0 alongside Cognito and AzureAD.
  evidence: https://github.com/luthersystems/lutherauth-sdk-go README; docs release-notes.md.
  name: lutherauth-jwt
  scheme: bearer
  type: http
- api: Luther Platform starter-kit middleware (sandbox oracle API)
  description: securityDefinitions.X-API-KEY in the grpc-gateway-generated oracle.swagger.json of the sandbox starter kit; the platform SDK also supports API-key pre-validation before claim extraction.
  evidence: https://github.com/luthersystems/sandbox/blob/main/api/srvpb/v1/oracle.swagger.json
  header: X-API-KEY
  in: header
  name: x-api-key
  type: apiKey
slug: luthersystems-com-authentication
source_filename: luthersystems-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://agentsearch.luthersystems.com/.well-known/agent-card.json (securitySchemes), the AgentSearch\n  OpenAPI (no securitySchemes), https://agentsearch.luthersystems.com/api-docs, the InsideOut SKILL.md,\n  AGENTS.md and SECURITY.md in https://github.com/luthersystems/insideout-agent-skills, live tools/list\n  descriptions (convoopen, credawait), the InsideOut A2A endpoint's -32602 X-A2A-Task-Secret response,\n  https://github.com/luthersystems/lutherauth-sdk-go and the sandbox starter kit's oracle.swagger.json.\n  derive-authentication.py produced no profile because the OpenAPI declares no securitySchemes.\ndescription: >-\n  Three distinct postures. AgentSearch is anonymous end to end — no keys, the card declares\n  securitySchemes.public.type \"none\". InsideOut is anonymous for design and pricing but session-scoped:\n  convoopen mints a session_id whose ?token= suffix is the per-session credential, deployment requires\
  \ the\n  user to connect AWS/GCP credentials in a browser (the cloud provider's own OAuth, never passed through\n  the agent) and to subscribe, and the A2A tasks/get method requires an X-A2A-Task-Secret header. The\n  Luther Enterprise platform (customer-deployed) authenticates with RS256 JWTs issued by LutherAuth against\n  external OIDC IdPs (Cognito, AzureAD, Auth0), with API-key pre-validation supported by the Go SDK and an\n  X-API-KEY header on the starter-kit middleware API.\nschemes:\n- name: public\n  api: AgentSearch (HTTP, MCP, A2A)\n  type: none\n  description: All endpoints publicly readable; no credential of any kind. Rate limiting is per IP, best effort.\n  evidence: 'agent card securitySchemes.public is {\"type\":\"none\"}; OpenAPI has no securitySchemes/security; MCP initialize + tools/list answered anonymously.'\n- name: insideout-session-token\n  api: InsideOut MCP (https://app.luthersystems.com/v1/insideout-mcp)\n  type: bearer-in-session-id\n  description: convoopen\
  \ returns session_id in the form sess_v2_xxx?token=yyy; the token is part of the session id and must be sent verbatim on every later tool call. No user-supplied API key. Mcp-Session-Id header carries the MCP transport session.\n  scopes: none\n  evidence: convoopen tool description (live tools/list); SKILL.md \"No API keys required from the user\".\n- name: cloud-credential-connect\n  api: InsideOut MCP (tfdeploy, tfdestroy, awsinspect, gcpinspect)\n  type: delegated (browser-based cloud-provider OAuth, out of band)\n  description: Deployment and inspection need the user to open a connect URL, authenticate directly with AWS or GCP and subscribe to a Luther Systems plan; credawait polls for completion. Credentials are held by the InsideOut platform, never by the agent or skill.\n  evidence: credawait tool description; SECURITY.md \"Cloud credentials\" section.\n- name: x-a2a-task-secret\n  api: InsideOut A2A (https://insideout.luthersystems.com/insideout-a2a/v0/)\n  type: apiKey\n  in:\
  \ header\n  header: X-A2A-Task-Secret\n  description: Required by tasks/get; not declared in the card's securitySchemes.\n  evidence: 'live -32602 \"X-A2A-Task-Secret header is required: invalid params\".'\n- name: lutherauth-jwt\n  api: Luther Enterprise platform (customer-deployed middleware / gRPC)\n  type: http\n  scheme: bearer\n  bearer_format: JWT (RS256)\n  description: Tokens issued by LutherAuth after OAuth/OIDC login with an external IdP; validated from gRPC metadata, HTTP cookies or headers via lutherauth-sdk-go with JWK caching and CSRF nonces. LutherAuth v4.7.6 added Auth0 alongside Cognito and AzureAD.\n  evidence: https://github.com/luthersystems/lutherauth-sdk-go README; docs release-notes.md.\n- name: x-api-key\n  api: Luther Platform starter-kit middleware (sandbox oracle API)\n  type: apiKey\n  in: header\n  header: X-API-KEY\n  description: securityDefinitions.X-API-KEY in the grpc-gateway-generated oracle.swagger.json of the sandbox starter kit; the platform SDK also\
  \ supports API-key pre-validation before claim extraction.\n  evidence: https://github.com/luthersystems/sandbox/blob/main/api/srvpb/v1/oracle.swagger.json\ndocs: https://github.com/luthersystems/insideout-agent-skills/blob/main/SECURITY.md\noauth: false\noidc_discovery: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luthersystems-com/refs/heads/main/authentication/luthersystems-com-authentication.yml
summary_line: 6 schemes
tags:
- Agents
- Agent Discovery
- MCP
- A2A
- agent-native
- Cloud Infrastructure
- Terraform
- Infrastructure as Code
- Process Automation
- Enterprise Automation
- Distributed Ledger
- Hyperledger Fabric
- Insurance
- Financial-Services
- Open-Source
---
