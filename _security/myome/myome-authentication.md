---
api_key_in: []
api_specs:
- filename: myome-openapi.json
  format: json
  label: MyOme API
  slug: myome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myome/refs/heads/main/openapi/myome-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Myome Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyOme secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MyOme
provider_slug: myome
scheme_count: 1
schemes:
- applied_to: 'security: [{jwt: []}] is applied per-operation on 7 of the 8 publicly visible operations. GET /consent declares security: [] (empty), but the live gateway still refuses unauthenticated calls, so no operation is anonymously callable in practice.'
  bearerFormat: JWT
  credential_delivery: MyOme will provide credentials to partners via secure email during account creation. Those credentials should be kept confidential.
  description: JSON Web Token (JWT) obtained from Keycloak with partner-specific credentials.
  header: 'Authorization: Bearer <token>'
  issuer:
    evidence: 'The spec states "Client obtains JWT from auth.myome.com" and "a JWT generated using Keycloak with partner-specific credentials". Confirmed by probe: auth.myome.com answers with Keycloak/RESTEasy error bodies ("RESTEASY003210: Could not find resource for full path"), and https://auth.myome.com/health returns 200.'
    host: auth.myome.com
    oidc_discovery: null
    oidc_discovery_note: No OIDC discovery document is reachable anonymously. /.well-known/openid-configuration 404s at the host root, and /realms/<realm>/.well-known/ openid-configuration and /auth/realms/<realm>/.well-known/openid-configuration were probed for ten candidate realm names (myome, partner, partners, api, master, external, clients, myome-api, production, prod) — every one 404. The realm name is partner-private.
    product: Keycloak
  name: jwt
  scheme: bearer
  sources:
  - openapi/myome-openapi.json
  - https://api.myome.com/0/ui/
  token_lifetime: The token refreshes every hour.
  type: http
slug: myome-authentication
source_filename: myome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: 'openapi/myome-openapi.json (components.securitySchemes) enriched from the \"API Conventions >\n  Authorization\" section of the published API reference at https://api.myome.com/0/ui/ (HTTP 200),\n  plus live probes of api.myome.com and auth.myome.com on 2026-08-26.'\ndocs: https://api.myome.com/0/ui/\nsummary:\n  types:\n  - http\n  self_service: false\n  self_service_detail: 'There is no sign-up or key-issuance flow. MyOme provides partner-specific\n    credentials by secure email during account creation, so API access requires a partner relationship\n    established out of band.'\nschemes:\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer <token>'\n  description: 'JSON Web Token (JWT) obtained from Keycloak with partner-specific credentials.'\n  issuer:\n    host: auth.myome.com\n    product: Keycloak\n    evidence: 'The spec states \"Client obtains JWT from auth.myome.com\"\
  \ and \"a JWT generated using\n      Keycloak with partner-specific credentials\". Confirmed by probe: auth.myome.com answers with\n      Keycloak/RESTEasy error bodies (\"RESTEASY003210: Could not find resource for full path\"), and\n      https://auth.myome.com/health returns 200.'\n    oidc_discovery: null\n    oidc_discovery_note: 'No OIDC discovery document is reachable anonymously.\n      /.well-known/openid-configuration 404s at the host root, and /realms/<realm>/.well-known/\n      openid-configuration and /auth/realms/<realm>/.well-known/openid-configuration were probed for\n      ten candidate realm names (myome, partner, partners, api, master, external, clients, myome-api,\n      production, prod) — every one 404. The realm name is partner-private.'\n  token_lifetime: 'The token refreshes every hour.'\n  credential_delivery: 'MyOme will provide credentials to partners via secure email during account\n    creation. Those credentials should be kept confidential.'\n  applied_to:\
  \ 'security: [{jwt: []}] is applied per-operation on 7 of the 8 publicly visible\n    operations. GET /consent declares security: [] (empty), but the live gateway still refuses\n    unauthenticated calls, so no operation is anonymously callable in practice.'\n  sources:\n  - openapi/myome-openapi.json\n  - https://api.myome.com/0/ui/\noauth2:\n  present: false\n  scopes: []\n  note: 'No oauth2 securityScheme, no flows, no authorizationUrl/tokenUrl and no scope vocabulary are\n    declared. The grant used to mint the JWT at Keycloak is not described in the public contract, so\n    no scopes/ artifact is emitted — deriving one would be invention.'\napi_keys:\n  present: false\nmutual_tls:\n  present: false\nobserved:\n- url: https://api.myome.com/0/product\n  status: 401\n  body: '{\"type\": \"about:blank\", \"title\": \"Unauthorized\", \"detail\": \"No authorization token provided\", \"status\": 401}'\nnotes: 'Single-scheme, bearer-JWT auth with no scope model and no self-service issuance.\
  \ For an agent\n  this means access is all-or-nothing: a partner token carries whatever the partner account can do,\n  and there is no published way to mint a narrower credential for a read-only or single-purpose agent.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myome/refs/heads/main/authentication/myome-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Genomics
- Healthcare
- Clinical Laboratory
- Whole Genome Sequencing
- Precision Medicine
- Bioinformatics
- Polygenic Risk Scores
- Pharmacogenomics
- Rare Disease
- Diagnostics
- Life Sciences
---
