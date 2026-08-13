---
api_key_in: []
auth_types:
- none
- oauth2
- http
description: ''
kind: authentication
layout: security
method: probed
name: Droplet Biosciences Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Droplet Biosciences secures its APIs with none, oauth2, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Droplet Biosciences
provider_slug: droplet-biosciences
scheme_count: 3
schemes:
- applies_to:
  - https://dropletbiosci.com/wp-json/wp/v2/*
  description: Published content collections (posts, pages, media, and the custom types publications, press-releases, team) return 200 with no credential. Verified 2026-08-12.
  name: anonymous
  sources:
  - https://dropletbiosci.com/wp-json/wp/v2/publications
  type: none
- applies_to:
  - https://dropletbiosci.com/wp-json/mcp/*
  - https://dropletbiosci.com/wp-json/wp-abilities/v1/*
  client_authentication:
    note: Public clients only — no confidential-client authentication method is advertised.
    token_endpoint_auth_methods_supported:
    - none
  discovery:
    metadata_url: https://dropletbiosci.com/wp-json/oauth/v1/metadata
    note: Metadata is NOT served at /.well-known/oauth-authorization-server (404), so a standards- compliant RFC 8414 client will fail discovery against this issuer.
    rfc8414_well_known: false
  dynamic_client_registration:
    note: Open registration endpoint; not exercised by this probe (registering a client would write to the provider's system).
    spec: RFC 7591
    supported: true
    url: https://dropletbiosci.com/wp-json/oauth/v1/register
  flows:
  - authorizationUrl: https://dropletbiosci.com/events-manager/oauth/authorize
    flow: authorizationCode
    issuer: https://dropletbiosci.com/events-manager
    registrationUrl: https://dropletbiosci.com/wp-json/oauth/v1/register
    revocationUrl: https://dropletbiosci.com/wp-json/oauth/v1/revoke
    scopes:
      events-manager:mcp: Access the Events Manager MCP server
    tokenUrl: https://dropletbiosci.com/wp-json/oauth/v1/token
  jwks:
    keys: 0
    note: The JWKS document is served but empty ({"keys":[]}), so no token signature can be verified from published material.
    status: 200
    url: https://dropletbiosci.com/wp-json/oauth/v1/jwks
  name: oauth2
  pkce:
    code_challenge_methods_supported:
    - S256
    required: true
  sources:
  - https://dropletbiosci.com/wp-json/oauth/v1/metadata
  type: oauth2
- applies_to:
  - https://dropletbiosci.com/wp-json/wp/v2/*
  description: WordPress application passwords, advertised in the /wp-json/ discovery document's authentication block. Authorization is granted interactively at https://dropletbiosci.com/wp-admin/authorize-application.php. Write access only; there is no self-service developer signup behind it.
  name: application-passwords
  scheme: basic
  sources:
  - https://dropletbiosci.com/wp-json/
  type: http
slug: droplet-biosciences-authentication
source_filename: droplet-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://dropletbiosci.com/wp-json/oauth/v1/metadata\nnote: >-\n  Derived from live, anonymously readable discovery documents on dropletbiosci.com — there is no\n  OpenAPI to derive from and the provider publishes no authentication documentation page. Two\n  distinct auth models coexist on the same host: the WordPress core REST API is READ-ANONYMOUS\n  for published content and uses cookie+nonce or application passwords for writes, while the MCP\n  and Abilities surfaces sit behind an OAuth 2.0 authorization server. None of this is a Droplet\n  developer program; it is the auth posture of the CMS the company runs its marketing site on.\nsummary:\n  types: [none, oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_read: true\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - https://dropletbiosci.com/wp-json/wp/v2/*\n  description: >-\n    Published content collections (posts, pages, media,\
  \ and the custom types publications,\n    press-releases, team) return 200 with no credential. Verified 2026-08-12.\n  sources: [https://dropletbiosci.com/wp-json/wp/v2/publications]\n- name: oauth2\n  type: oauth2\n  applies_to:\n  - https://dropletbiosci.com/wp-json/mcp/*\n  - https://dropletbiosci.com/wp-json/wp-abilities/v1/*\n  flows:\n  - flow: authorizationCode\n    issuer: https://dropletbiosci.com/events-manager\n    authorizationUrl: https://dropletbiosci.com/events-manager/oauth/authorize\n    tokenUrl: https://dropletbiosci.com/wp-json/oauth/v1/token\n    revocationUrl: https://dropletbiosci.com/wp-json/oauth/v1/revoke\n    registrationUrl: https://dropletbiosci.com/wp-json/oauth/v1/register\n    scopes:\n      events-manager:mcp: Access the Events Manager MCP server\n  pkce:\n    required: true\n    code_challenge_methods_supported: [S256]\n  client_authentication:\n    token_endpoint_auth_methods_supported: [none]\n    note: Public clients only — no confidential-client authentication\
  \ method is advertised.\n  dynamic_client_registration:\n    supported: true\n    spec: RFC 7591\n    url: https://dropletbiosci.com/wp-json/oauth/v1/register\n    note: Open registration endpoint; not exercised by this probe (registering a client would write to the provider's system).\n  jwks:\n    url: https://dropletbiosci.com/wp-json/oauth/v1/jwks\n    status: 200\n    keys: 0\n    note: 'The JWKS document is served but empty ({\"keys\":[]}), so no token signature can be verified from published material.'\n  discovery:\n    metadata_url: https://dropletbiosci.com/wp-json/oauth/v1/metadata\n    rfc8414_well_known: false\n    note: >-\n      Metadata is NOT served at /.well-known/oauth-authorization-server (404), so a standards-\n      compliant RFC 8414 client will fail discovery against this issuer.\n  sources: [https://dropletbiosci.com/wp-json/oauth/v1/metadata]\n- name: application-passwords\n  type: http\n  scheme: basic\n  applies_to:\n  - https://dropletbiosci.com/wp-json/wp/v2/*\n\
  \  description: >-\n    WordPress application passwords, advertised in the /wp-json/ discovery document's\n    authentication block. Authorization is granted interactively at\n    https://dropletbiosci.com/wp-admin/authorize-application.php. Write access only; there is no\n    self-service developer signup behind it.\n  sources: [https://dropletbiosci.com/wp-json/]\ngaps:\n- No authentication documentation page exists on the provider's site.\n- No RFC 8414 or RFC 9728 well-known discovery.\n- Empty JWKS.\n- The 401 challenge carries no WWW-Authenticate header pointing at the authorization server.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - {url: 'https://dropletbiosci.com/wp-json/oauth/v1/metadata', http_status: 200}\n  - {url: 'https://dropletbiosci.com/wp-json/oauth/v1/jwks', http_status: 200}\n  - {url: 'https://dropletbiosci.com/.well-known/oauth-authorization-server', http_status: 404}\n  - {url: 'https://dropletbiosci.com/.well-known/oauth-protected-resource', http_status:\
  \ 404}\n  - {url: 'https://dropletbiosci.com/wp-json/wp/v2/publications?per_page=1', http_status: 200}\n  - {url: 'https://dropletbiosci.com/wp-json/wp-abilities/v1/abilities', http_status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/droplet-biosciences/refs/heads/main/authentication/droplet-biosciences-authentication.yml
summary_line: none/oauth2/http · 3 schemes
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Oncology
- Genomics
- Liquid Biopsy
- Life Sciences
- Biotechnology
- Clinical Laboratory
---
