---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cardless Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Cardless secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Cardless
provider_slug: cardless
scheme_count: 3
schemes:
- applies_to: cardless:partner-api
  description: Partner token exchange is protected with HTTP Basic authentication. The username is a fixed partner client identifier; the password is issued to the partner during onboarding. Credentials are not self-service — there is no public sign-up for API credentials.
  name: partnerBasicAuth
  scheme: basic
  sources:
  - docs.cardless.com partner authentication reference
  type: http
- applies_to: cardless:partner-api
  bearerFormat: JWT
  description: 'All servicing requests carry a bearer access token obtained from the partner token endpoint. The token grant is partner-scoped: the partner presents a JWT signed with its own partner key together with the partner user identifier, and receives a short-lived access token plus a refresh token. The token response also returns the Cardless user identifier and the list of account identifiers the partner user may act on, so authorization is account-scoped rather than scope-string-scoped.'
  grant_types:
  - partner
  - refresh_token
  name: partnerBearerToken
  scheme: bearer
  sources:
  - docs.cardless.com partner authentication reference
  token_lifetime_seconds: 3599
  type: http
- applies_to: cardless:docs-mcp
  description: 'OAuth 2.0 for the documentation MCP server, advertised via RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata. Supports dynamic client registration (RFC 7591) and PKCE S256. One scope: mcp:search. tools/list and tools/call are currently answered anonymously as well.'
  flows:
  - authorizationUrl: https://docs.cardless.com/mcp/oauth/authorize
    flow: authorizationCode
    scopes:
    - mcp:search
    tokenUrl: https://docs.cardless.com/mcp/oauth/token
  - flow: clientCredentials
    scopes:
    - mcp:search
    tokenUrl: https://docs.cardless.com/mcp/oauth/token
  issuer: https://docs.cardless.com/mcp/oauth
  name: docsMcpOAuth
  sources:
  - well-known/cardless-oauth-authorization-server.json
  type: oauth2
slug: cardless-authentication
source_filename: cardless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: 'docs.cardless.com partner authentication reference (partner-gated) + https://docs.cardless.com/.well-known/oauth-authorization-server'\ndocs: https://docs.cardless.com/\nx-docs-access: partner-gated\nsummary:\n  types: [http, oauth2]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  api_key_in: []\n  delegated_consent: false\nschemes:\n- name: partnerBasicAuth\n  type: http\n  scheme: basic\n  applies_to: cardless:partner-api\n  description: 'Partner token exchange is protected with HTTP Basic authentication.\n    The username is a fixed partner client identifier; the password is issued to the\n    partner during onboarding. Credentials are not self-service — there is no public\n    sign-up for API credentials.'\n  sources: ['docs.cardless.com partner authentication reference']\n- name: partnerBearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to:\
  \ cardless:partner-api\n  description: 'All servicing requests carry a bearer access token obtained from the\n    partner token endpoint. The token grant is partner-scoped: the partner presents a\n    JWT signed with its own partner key together with the partner user identifier, and\n    receives a short-lived access token plus a refresh token. The token response also\n    returns the Cardless user identifier and the list of account identifiers the partner\n    user may act on, so authorization is account-scoped rather than scope-string-scoped.'\n  grant_types: [partner, refresh_token]\n  token_lifetime_seconds: 3599\n  sources: ['docs.cardless.com partner authentication reference']\n- name: docsMcpOAuth\n  type: oauth2\n  applies_to: cardless:docs-mcp\n  description: 'OAuth 2.0 for the documentation MCP server, advertised via RFC 8414\n    authorization-server metadata and RFC 9728 protected-resource metadata. Supports\n    dynamic client registration (RFC 7591) and PKCE S256. One scope:\
  \ mcp:search.\n    tools/list and tools/call are currently answered anonymously as well.'\n  issuer: https://docs.cardless.com/mcp/oauth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docs.cardless.com/mcp/oauth/authorize\n    tokenUrl: https://docs.cardless.com/mcp/oauth/token\n    scopes: [mcp:search]\n  - flow: clientCredentials\n    tokenUrl: https://docs.cardless.com/mcp/oauth/token\n    scopes: [mcp:search]\n  sources: [well-known/cardless-oauth-authorization-server.json]\nnotes:\n- 'No public API keys, no self-service credential issuance, no public sandbox credentials.\n  Cardless is a partner-onboarded platform: API access is granted through a commercial\n  onboarding process.'\n- 'No OpenAPI document is published on any public Cardless host; the specification\n  fragments that back the documentation are behind the partner login.'\nx-evidence:\n  fetched: '2026-08-01'\n  hosts_probed: [api.cardless.com, docs.cardless.com, www.cardless.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardless/refs/heads/main/authentication/cardless-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Financial Services
- Fintech
- Credit Cards
- Card Issuing
- Embedded Finance
- Payments
- Banking as a Service
- Lending
- Co-Branded Cards
- Loyalty
---
