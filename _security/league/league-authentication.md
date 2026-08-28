---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: League Authentication
name_suffix: Authentication
oauth_flows: []
overview: League declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: League
provider_slug: league
scheme_count: 1
schemes:
- description: The Developer Program Terms state that "Customers receive provisioned API Keys for authorized use cases" and that League "may monitor Customer's use of any API by the Customer Developed Apps through any technical means". The header or query parameter carrying the key is not published.
  evidence: https://league.com/developer-program-terms/
  in: unknown
  method: searched
  name: API Key
  provisioning: Per-customer, per-use-case. Annex 1 of the terms currently authorizes a single use case, "Embedding into Existing Applications".
  type: apiKey
slug: league-authentication
source_filename: league-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://league.com/developer-program-terms/\nname: League Platform API authentication\nprovider: League\nsummary: >-\n  League provisions API Keys to contracted customers under the Developer Program Terms. There is no\n  public authentication reference, no OpenAPI securitySchemes to derive from, and no OAuth or OIDC\n  discovery document served on any League host.\nschemes:\n- type: apiKey\n  name: API Key\n  in: unknown\n  description: >-\n    The Developer Program Terms state that \"Customers receive provisioned API Keys for authorized use\n    cases\" and that League \"may monitor Customer's use of any API by the Customer Developed Apps\n    through any technical means\". The header or query parameter carrying the key is not published.\n  method: searched\n  evidence: https://league.com/developer-program-terms/\n  provisioning: >-\n    Per-customer, per-use-case. Annex 1 of the terms currently authorizes a single use case,\n\
  \    \"Embedding into Existing Applications\".\noauth:\n  present: false\n  note: >-\n    No OAuth 2.0 or OpenID Connect surface is discoverable. Probed and all missed:\n    api.league.com/.well-known/oauth-authorization-server (404),\n    api.league.com/.well-known/oauth-protected-resource (404),\n    api.league.com/.well-known/openid-configuration (404),\n    app.league.com/.well-known/openid-configuration (404).\n    League's own documentation portal is fronted by Auth0\n    (documentation-portal.leagueinc-prod-usa.auth0.com) but that is League's internal IdP for docs\n    access, not an API authorization server exposed to integrators.\nobserved_behaviour:\n  note: >-\n    The gateway does not challenge. Every unauthenticated request to api.league.com returns 404 with a\n    JSON:API error document rather than 401 with a WWW-Authenticate header, so the auth scheme cannot\n    be probed anonymously and unentitled routes are indistinguishable from absent ones.\n  www_authenticate_observed:\
  \ false\n  probed: '2026-08-25'\nmtls:\n  present: unknown\ndocs: null\ndocs_note: >-\n  The authentication reference is inside the customer documentation portal. https://docs.league.com/\n  302s to an Auth0 universal login (HTTP 400 at the login endpoint for an anonymous client).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/league/refs/heads/main/authentication/league-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Health
- Healthcare
- Digital Health
- Health Benefits
- Interoperability
- FHIR
- Agents
- Artificial Intelligence
- Patient Engagement
- Insurance
- SaaS
---
