---
anonymous_access: false
api_key_in: []
auth_types: []
description: CloudEagle publishes no OpenAPI and no public developer reference, so this profile is built from the discovery documents CloudEagle actually serves and from live probes of its API host — not from a specification. Two distinct authenticated surfaces exist and they do NOT share an auth model.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Cloudeagle Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudEagle.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CloudEagle.ai
provider_slug: cloudeagle
scheme_count: 2
schemes:
- authorization_endpoint: https://mcp.cloudeagle.ai/authorize
  bearer_note: 'The 401 carries no WWW-Authenticate header, so the expected bearer presentation method is not advertised. RFC 6750 Authorization: Bearer is the reasonable assumption but was NOT confirmed and is not asserted.'
  bearer_transport: unconfirmed
  client_authentication: none
  client_type: public
  dynamic_client_registration: true
  evidence:
  - http_status: 200
    url: https://mcp.cloudeagle.ai/.well-known/oauth-authorization-server
  - http_status: 200
    url: https://mcp.cloudeagle.ai/.well-known/oauth-protected-resource
  - http_status: 200
    url: https://mcp.cloudeagle.ai/authorize
  flow: authorizationCode
  id: mcp-oauth2
  issuer: https://mcp.cloudeagle.ai
  pkce:
    methods:
    - S256
    required: true
  registration_endpoint: https://mcp.cloudeagle.ai/register
  scopes: []
  scopes_note: The authorization-server metadata advertises no scopes_supported and CloudEagle documents no permission model. An integrator cannot request least-privilege access; the grant appears to be all-or-nothing at tenant level.
  surface: CloudEagle.ai MCP Server (https://mcp.cloudeagle.ai)
  tenant_binding: Authorization begins with a tenant chooser — /authorize asks for the subdomain the operator signs in with (e.g. acme from acme.cloudeagle.ai) — so a token is scoped to one CloudEagle tenant.
  token_endpoint: https://mcp.cloudeagle.ai/token
  type: oauth2
- description: CloudEagle states that the MCP connector is authorised "with an API token generated from your CloudEagle tenant", which is the only public statement about how the REST surface is credentialled. The header or parameter the token is presented in is NOT published and was NOT confirmed — nothing is asserted about it here.
  evidence:
  - http_status: 401
    note: Returns {"status":401,"message":"Not authorized","data":"Not authorized", "requestId":null}. A control path that does not exist (/zzz-does-not-exist-9876) returns the identical 401, so the host denies everything anonymously and reveals no scheme.
    url: https://api.cloudeagle.ai/
  - http_status: 200
    note: '"Authorize with an API token generated from your CloudEagle tenant."'
    url: https://www.cloudeagle.ai/blogs/mcp-server-saas-ai-identity-insights
  id: enterprise-api-token
  in: unconfirmed
  key_issuance: In-product, per tenant. Not self-service on a public developer portal.
  name: unconfirmed
  surface: CloudEagle enterprise REST API (https://api.cloudeagle.ai)
  type: apiKey
slug: cloudeagle-authentication
source_filename: cloudeagle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://mcp.cloudeagle.ai/.well-known/oauth-authorization-server +\n  https://mcp.cloudeagle.ai/.well-known/oauth-protected-resource +\n  live probes of https://api.cloudeagle.ai/ +\n  https://www.cloudeagle.ai/blogs/mcp-server-saas-ai-identity-insights\nprovider: CloudEagle.ai\nproviderId: cloudeagle\ndescription: >-\n  CloudEagle publishes no OpenAPI and no public developer reference, so this\n  profile is built from the discovery documents CloudEagle actually serves and\n  from live probes of its API host — not from a specification. Two distinct\n  authenticated surfaces exist and they do NOT share an auth model.\n\nschemes:\n\n- id: mcp-oauth2\n  surface: CloudEagle.ai MCP Server (https://mcp.cloudeagle.ai)\n  type: oauth2\n  flow: authorizationCode\n  pkce:\n    required: true\n    methods: [S256]\n  issuer: https://mcp.cloudeagle.ai\n  authorization_endpoint: https://mcp.cloudeagle.ai/authorize\n  token_endpoint:\
  \ https://mcp.cloudeagle.ai/token\n  registration_endpoint: https://mcp.cloudeagle.ai/register\n  dynamic_client_registration: true\n  client_authentication: none\n  client_type: public\n  scopes: []\n  scopes_note: >-\n    The authorization-server metadata advertises no scopes_supported and\n    CloudEagle documents no permission model. An integrator cannot request\n    least-privilege access; the grant appears to be all-or-nothing at tenant\n    level.\n  bearer_transport: unconfirmed\n  bearer_note: >-\n    The 401 carries no WWW-Authenticate header, so the expected bearer\n    presentation method is not advertised. RFC 6750 Authorization: Bearer is the\n    reasonable assumption but was NOT confirmed and is not asserted.\n  tenant_binding: >-\n    Authorization begins with a tenant chooser — /authorize asks for the\n    subdomain the operator signs in with (e.g. acme from acme.cloudeagle.ai) —\n    so a token is scoped to one CloudEagle tenant.\n  evidence:\n  - url: https://mcp.cloudeagle.ai/.well-known/oauth-authorization-server\n\
  \    http_status: 200\n  - url: https://mcp.cloudeagle.ai/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://mcp.cloudeagle.ai/authorize\n    http_status: 200\n\n- id: enterprise-api-token\n  surface: CloudEagle enterprise REST API (https://api.cloudeagle.ai)\n  type: apiKey\n  in: unconfirmed\n  name: unconfirmed\n  description: >-\n    CloudEagle states that the MCP connector is authorised \"with an API token\n    generated from your CloudEagle tenant\", which is the only public statement\n    about how the REST surface is credentialled. The header or parameter the\n    token is presented in is NOT published and was NOT confirmed — nothing is\n    asserted about it here.\n  key_issuance: In-product, per tenant. Not self-service on a public developer portal.\n  evidence:\n  - url: https://api.cloudeagle.ai/\n    http_status: 401\n    note: >-\n      Returns {\"status\":401,\"message\":\"Not authorized\",\"data\":\"Not authorized\",\n      \"requestId\":null}.\
  \ A control path that does not exist\n      (/zzz-does-not-exist-9876) returns the identical 401, so the host denies\n      everything anonymously and reveals no scheme.\n  - url: https://www.cloudeagle.ai/blogs/mcp-server-saas-ai-identity-insights\n    http_status: 200\n    note: '\"Authorize with an API token generated from your CloudEagle tenant.\"'\n\nnot_found:\n- mutualTLS\n- openIdConnect\n- http-basic\n- http-bearer-documented\nopenid_connect_note: >-\n  mcp.cloudeagle.ai answers /.well-known/openid-configuration with a 200, but the\n  body is byte-identical to its OAuth 2.0 authorization-server metadata. There is\n  no jwks_uri, userinfo_endpoint, subject_types_supported or id_token_signing_alg,\n  so this is NOT an OpenID Connect provider and must not be treated as one.\n\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudeagle/refs/heads/main/authentication/cloudeagle-authentication.yml
summary_line: 2 schemes
tags:
- Access Governance
- Cost Optimization
- License Management
- Procurement
- SaaS Management
- Shadow AI
- Shadow IT
- Software Procurement
- Vendor Management
---
