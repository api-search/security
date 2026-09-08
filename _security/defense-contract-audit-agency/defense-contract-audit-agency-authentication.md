---
anonymous_access: true
api_key_in: []
auth_types:
- none
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Defense Contract Audit Agency Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Defense Contract Audit Agency secures its APIs with none and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Defense Contract Audit Agency
provider_slug: defense-contract-audit-agency
scheme_count: 2
schemes:
- applies_to: https://fao.dcaa.mil/api
  description: The DCAA Field Audit Office Branch Locator API answers unauthenticated GET requests. No Authorization header, API key, cookie or referer check was required for any of the six observed operations; responses carry only Strict-Transport-Security.
  evidence:
  - observed: '2026-09-07'
    status: 200
    url: https://fao.dcaa.mil/api/angularconfiguration/get-uei-regex
  - observed: '2026-09-07'
    status: 200
    url: https://fao.dcaa.mil/api/PublicBranch/search?searchCriteria=22060&searchType=2
  name: anonymous
  type: none
- applies_to: https://csp.dcaa.mil/
  authorization_server:
    discovery_document: none served — /.well-known/openid-configuration and /.well-known/oauth-authorization-server both returned 404 on piee.eb.mil (2026-09-07)
    first_party: false
    host: piee.eb.mil
    operator: DoD Procurement Integrated Enterprise Environment (PIEE)
  description: The DCAA Contractor Submission Portal (CSP) delegates sign-in to the DoD Procurement Integrated Enterprise Environment (PIEE). An unauthenticated request to any CSP path returns 302 to the PIEE authorization endpoint with the OAuth 2.0 authorization-code flow and PKCE (S256). DCAA operates the relying party; PIEE operates the authorization server. Credentials are DoD PIEE accounts (CAC/ECA), not developer keys.
  evidence:
  - observed: '2026-09-07'
    redirect_to: https://piee.eb.mil/portal/oauth2/authorize?client_id=csp&redirect_uri=https%3A%2F%2Fcsp.dcaa.mil%2Fsignin-oidc&response_type=code&scope=openid%20profile&code_challenge_method=S256
    status: 302
    url: https://csp.dcaa.mil/
  flows:
  - authorizationUrl: https://piee.eb.mil/portal/oauth2/authorize
    client_id: csp
    flow: authorizationCode
    pkce: S256
    redirect_uri: https://csp.dcaa.mil/signin-oidc
    scopes:
    - openid
    - profile
    tokenUrl: null
  name: piee-oidc
  type: openIdConnect
slug: defense-contract-audit-agency-authentication
source_filename: defense-contract-audit-agency-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  live HTTP probes 2026-09-07 of https://fao.dcaa.mil/api and https://csp.dcaa.mil/ —\n  DCAA publishes no OpenAPI, so there are no securitySchemes to derive from; every field\n  below was observed on the wire.\nnote: >-\n  Two distinct DCAA surfaces with two distinct auth models. The public Branch Locator API\n  is anonymous. The Contractor Submission Portal is federated to DoD PIEE over OpenID\n  Connect. There is no developer-facing authentication documentation of any kind — no API\n  keys, no client registration, no token endpoint DCAA operates itself.\nsummary:\n  types: [none, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: anonymous\n    type: none\n    applies_to: https://fao.dcaa.mil/api\n    description: >-\n      The DCAA Field Audit Office Branch Locator API answers unauthenticated GET requests.\n      No Authorization header, API key, cookie or referer check was required\
  \ for any of the\n      six observed operations; responses carry only Strict-Transport-Security.\n    evidence:\n      - url: https://fao.dcaa.mil/api/angularconfiguration/get-uei-regex\n        status: 200\n        observed: '2026-09-07'\n      - url: https://fao.dcaa.mil/api/PublicBranch/search?searchCriteria=22060&searchType=2\n        status: 200\n        observed: '2026-09-07'\n  - name: piee-oidc\n    type: openIdConnect\n    applies_to: https://csp.dcaa.mil/\n    description: >-\n      The DCAA Contractor Submission Portal (CSP) delegates sign-in to the DoD Procurement\n      Integrated Enterprise Environment (PIEE). An unauthenticated request to any CSP path\n      returns 302 to the PIEE authorization endpoint with the OAuth 2.0 authorization-code\n      flow and PKCE (S256). DCAA operates the relying party; PIEE operates the\n      authorization server. Credentials are DoD PIEE accounts (CAC/ECA), not developer keys.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://piee.eb.mil/portal/oauth2/authorize\n        tokenUrl: null\n        pkce: S256\n        client_id: csp\n        redirect_uri: https://csp.dcaa.mil/signin-oidc\n        scopes: [openid, profile]\n    authorization_server:\n      host: piee.eb.mil\n      operator: DoD Procurement Integrated Enterprise Environment (PIEE)\n      first_party: false\n      discovery_document: >-\n        none served — /.well-known/openid-configuration and\n        /.well-known/oauth-authorization-server both returned 404 on piee.eb.mil (2026-09-07)\n    evidence:\n      - url: https://csp.dcaa.mil/\n        status: 302\n        redirect_to: https://piee.eb.mil/portal/oauth2/authorize?client_id=csp&redirect_uri=https%3A%2F%2Fcsp.dcaa.mil%2Fsignin-oidc&response_type=code&scope=openid%20profile&code_challenge_method=S256\n        observed: '2026-09-07'\ndocs: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-contract-audit-agency/refs/heads/main/authentication/defense-contract-audit-agency-authentication.yml
summary_line: none/openIdConnect · 2 schemes
tags:
- Federal-Government
- Defense
- Department of Defense
- Audit
- Contract Audit
- Financial
- Government Contracting
- CAGE Code
- Unique Entity Identifier
- Locator
---
