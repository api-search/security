---
anonymous_access: true
api_key_in:
- header
auth_types:
- oauth2
- http-bearer
- none
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Rosentic Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Rosentic secures its APIs with oauth2, http-bearer, and none across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Rosentic
provider_slug: rosentic-com
scheme_count: 4
schemes:
- applies_to:
  - https://api.rosentic.com/mcp
  discovery:
    authorization_server: well-known/rosentic-com-oauth-authorization-server.json
    challenge: 'HTTP 401 with WWW-Authenticate: Bearer resource_metadata="https://api.rosentic.com/.well-known/oauth-protected-resource/mcp", scope="rosentic:remote:read"'
    protected_resource: well-known/rosentic-com-oauth-protected-resource.json
  flows:
  - authorizationUrl: https://api.rosentic.com/oauth/authorize
    flow: authorizationCode
    scopes:
      rosentic:remote:read: Read the hosted run_status / which_lane / get_verdict tools
    tokenUrl: https://api.rosentic.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: RosenticRemoteOAuth
  observed:
  - body: '{"error":"invalid_request","error_description":"response_type must be code"}'
    http_status: 400
    method: GET
    url: https://api.rosentic.com/oauth/authorize
  - body: '{}'
    body_out: '{"error":"invalid_client_metadata","error_description":"redirect_uris must contain 1 to 10 HTTPS or loopback HTTP URIs without fragments"}'
    http_status: 400
    method: POST
    url: https://api.rosentic.com/oauth/register
  pkce: S256 (required for the public client — token_endpoint_auth_methods_supported is [none])
  registration_endpoint: https://api.rosentic.com/oauth/register
  sources:
  - well-known/rosentic-com-oauth-authorization-server.json
  - 'https://rosentic.com/llms.txt — "Hosted MCP endpoint: https://api.rosentic.com/mcp (OAuth 2.1, PKCE, dynamic client registration)"'
  type: oauth2
- applies_to:
  - https://api.rosentic.com/mcp (alternative to OAuth per the 401 body)
  - GET https://api.rosentic.com/v1/feed/rules
  - MCP local tools get_verdict and get_remediation_queue
  - GitHub Action input api-key / env ROSENTIC_API_KEY (turns on dashboard history)
  - A2A bearer scheme for private repos, higher limits, Merge Index
  bearerFormat: Rosentic workspace API key, prefix ros_live_
  in: header
  issuance:
    cost: free (Free-with-key tier — 3 repos, 1,000 scans/month, 30-day history)
    how: Sign in with GitHub (read:org read:user user:email) or a magic-link email, select an org to create a workspace, install the GitHub App or "claim without installing"; "This secret was returned by the claim and is shown once."
    where: https://api.rosentic.com/onboard
  name: RosenticApiKey
  parameter: 'Authorization: Bearer <ROSENTIC_API_KEY>'
  scheme: bearer
  sources:
  - https://rosentic.com/docs/ — Enable dashboard history
  - 'https://rosentic.com/docs/integrations/ — curl https://api.rosentic.com/v1/feed/rules -H "Authorization: Bearer $ROSENTIC_API_KEY"'
  - https://pypi.org/project/rosentic-mcp/ — get_verdict "Requires ROSENTIC_API_KEY (a ros_live_ workspace key)"
  - MCP 401 body next_step
  type: http
- applies_to:
  - A2A skills on public repos — "Public repos, 3 requests/hour per IP, 250MB repo cap" (agent card authentication.schemes[0])
  - GitHub Action in anonymous mode (uses the runner's GITHUB_TOKEN only)
  - The six offline MCP tools and rosentic-mcp gate
  - get_policy — "Public read - no key needed"
  name: Anonymous
  sources:
  - a2a/rosentic-com-agent-card.json
  - https://github.com/Rosentic/rosentic-action README — "No signup. No API key. No account."
  type: none
- applies_to:
  - https://api.rosentic.com/auth/github
  audience: dashboard sign-in, not API auth
  name: GitHubOAuthSignIn
  note: Delegates identity to GitHub; "No write access requested" (onboard page). Email magic link is the alternative. Produces a dashboard session, which the MCP 401 body also accepts.
  observed:
    http_status: 302
    location: https://github.com/login/oauth/authorize?client_id=Ov23lipUElad6nbA4R9W&redirect_uri=https%3A%2F%2Fapi.rosentic.com%2Fauth%2Fgithub%2Fcallback&scope=read%3Aorg+read%3Auser+user%3Aemail&state=...
  type: oauth2
slug: rosentic-com-authentication
source_filename: rosentic-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.rosentic.com/.well-known/oauth-authorization-server\ndocs:\n- https://rosentic.com/mcp/\n- https://rosentic.com/docs/\n- https://rosentic.com/docs/integrations/\n- https://api.rosentic.com/onboard\n- https://pypi.org/project/rosentic-mcp/\nsummary:\n  types: [oauth2, http-bearer, none]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  bearer: true\n  pkce: S256\n  dynamic_client_registration: true\n  credential_classes: 4\n  headline: >-\n    Four ways in, by surface. (1) Rosentic Remote MCP at https://api.rosentic.com/mcp: OAuth 2.1\n    authorization-code with PKCE S256 for a public client, dynamic client registration, one scope\n    rosentic:remote:read — discovered through the RFC 9728 / RFC 8414 chain the endpoint's 401 points at —\n    or a Rosentic API key as a Bearer token. (2) The REST feed and the dashboard-backed MCP tools: a\n    workspace API key (ros_live_ prefix) as Authorization: Bearer,\
  \ issued once at onboarding. (3) The A2A\n    agent: anonymous for public repos (3 requests/hour per IP, 250MB repo cap) or Bearer API key for\n    private repos and Merge Index. (4) The GitHub Action and the six offline MCP tools: no credential at\n    all — \"No signup. No API key. No account.\" No OIDC is served (/.well-known/openid-configuration 404),\n    and no OpenAPI declares any of this, so derive-authentication.py had nothing to read.\nschemes:\n- name: RosenticRemoteOAuth\n  type: oauth2\n  applies_to: [https://api.rosentic.com/mcp]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.rosentic.com/oauth/authorize\n    tokenUrl: https://api.rosentic.com/oauth/token\n    scopes: {rosentic:remote:read: Read the hosted run_status / which_lane / get_verdict tools}\n  pkce: S256 (required for the public client — token_endpoint_auth_methods_supported is [none])\n  grant_types: [authorization_code, refresh_token]\n  registration_endpoint: https://api.rosentic.com/oauth/register\n\
  \  discovery:\n    authorization_server: well-known/rosentic-com-oauth-authorization-server.json\n    protected_resource: well-known/rosentic-com-oauth-protected-resource.json\n    challenge: 'HTTP 401 with WWW-Authenticate: Bearer resource_metadata=\"https://api.rosentic.com/.well-known/oauth-protected-resource/mcp\", scope=\"rosentic:remote:read\"'\n  observed:\n  - {url: 'https://api.rosentic.com/oauth/authorize', method: GET, http_status: 400, body: '{\"error\":\"invalid_request\",\"error_description\":\"response_type must be code\"}'}\n  - {url: 'https://api.rosentic.com/oauth/register', method: POST, body: '{}', http_status: 400, body_out: '{\"error\":\"invalid_client_metadata\",\"error_description\":\"redirect_uris must contain 1 to 10 HTTPS or loopback HTTP URIs without fragments\"}'}\n  sources: [well-known/rosentic-com-oauth-authorization-server.json, 'https://rosentic.com/llms.txt — \"Hosted MCP endpoint: https://api.rosentic.com/mcp (OAuth 2.1, PKCE, dynamic client registration)\"\
  ']\n- name: RosenticApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: 'Rosentic workspace API key, prefix ros_live_'\n  in: header\n  parameter: 'Authorization: Bearer <ROSENTIC_API_KEY>'\n  applies_to: ['https://api.rosentic.com/mcp (alternative to OAuth per the 401 body)', 'GET https://api.rosentic.com/v1/feed/rules', 'MCP local tools get_verdict and get_remediation_queue', 'GitHub Action input api-key / env ROSENTIC_API_KEY (turns on dashboard history)', 'A2A bearer scheme for private repos, higher limits, Merge Index']\n  issuance:\n    where: https://api.rosentic.com/onboard\n    how: 'Sign in with GitHub (read:org read:user user:email) or a magic-link email, select an org to create a workspace, install the GitHub App or \"claim without installing\"; \"This secret was returned by the claim and is shown once.\"'\n    cost: free (Free-with-key tier — 3 repos, 1,000 scans/month, 30-day history)\n  sources: ['https://rosentic.com/docs/ — Enable dashboard history', 'https://rosentic.com/docs/integrations/\
  \ — curl https://api.rosentic.com/v1/feed/rules -H \"Authorization: Bearer $ROSENTIC_API_KEY\"', 'https://pypi.org/project/rosentic-mcp/ — get_verdict \"Requires ROSENTIC_API_KEY (a ros_live_ workspace key)\"', 'MCP 401 body next_step']\n- name: Anonymous\n  type: none\n  applies_to: ['A2A skills on public repos — \"Public repos, 3 requests/hour per IP, 250MB repo cap\" (agent card authentication.schemes[0])', 'GitHub Action in anonymous mode (uses the runner''s GITHUB_TOKEN only)', 'The six offline MCP tools and rosentic-mcp gate', 'get_policy — \"Public read - no key needed\"']\n  sources: [a2a/rosentic-com-agent-card.json, 'https://github.com/Rosentic/rosentic-action README — \"No signup. No API key. No account.\"']\n- name: GitHubOAuthSignIn\n  type: oauth2\n  audience: dashboard sign-in, not API auth\n  applies_to: [https://api.rosentic.com/auth/github]\n  observed: {http_status: 302, location: 'https://github.com/login/oauth/authorize?client_id=Ov23lipUElad6nbA4R9W&redirect_uri=https%3A%2F%2Fapi.rosentic.com%2Fauth%2Fgithub%2Fcallback&scope=read%3Aorg+read%3Auser+user%3Aemail&state=...'}\n\
  \  note: Delegates identity to GitHub; \"No write access requested\" (onboard page). Email magic link is the alternative. Produces a dashboard session, which the MCP 401 body also accepts.\ngaps:\n- The A2A card carries its auth in the legacy authentication.schemes[] block rather than securitySchemes/security (see a2a/rosentic-com-a2a.yml deviations).\n- The OAuth metadata's resource_documentation and the 401 body's docs_url both point at github.com/Rosentic/rosentic/blob/main/docs/remote.md, which is not publicly readable (404); the readable remote docs are https://rosentic.com/mcp/.\n- GET https://api.rosentic.com/v1/feed/rules without a key returns the host's generic 404 ({\"error\":\"not_found\"}) rather than the documented 401 unauthorized, so an unauthenticated client cannot tell the endpoint exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rosentic-com/refs/heads/main/authentication/rosentic-com-authentication.yml
summary_line: oauth2/http-bearer/none · 4 schemes
tags:
- Developer Tools
- CI/CD
- Git
- Static Analysis
- Merge Safety
- AI Coding Agents
- MCP
- A2A
- GitHub Actions
- agent-native
---
