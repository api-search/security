---
api_key_in: []
api_specs:
- filename: university-of-the-witwatersrand-root-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Root API
  slug: university-of-the-witwatersrand-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-root-api-openapi.yml
- filename: university-of-the-witwatersrand-communities-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Communities API
  slug: university-of-the-witwatersrand-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-communities-api-openapi.yml
- filename: university-of-the-witwatersrand-collections-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Collections API
  slug: university-of-the-witwatersrand-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-collections-api-openapi.yml
- filename: university-of-the-witwatersrand-items-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Items API
  slug: university-of-the-witwatersrand-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-items-api-openapi.yml
- filename: university-of-the-witwatersrand-discovery-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Discovery API
  slug: university-of-the-witwatersrand-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-discovery-api-openapi.yml
- filename: university-of-the-witwatersrand-request-api-openapi.yml
  format: yaml
  label: WIReDSpace OAI-PMH Interface
  slug: university-of-the-witwatersrand-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-request-api-openapi.yml
auth_types:
- none
- session
description: 'Authentication posture of the institution-operated WIReDSpace surfaces only. The previous version of this file was derived from the Figshare v2 OAuth contract (authorizationUrl https://figshare.com/account/applications/authorize, tokenUrl https://api.figshare.com/v2/token) and therefore described the vendor''s authorization server, not the university''s — it was removed on 2026-08-30 together with the vendor spec it came from. WIReDSpace read access is anonymous: the DSpace 9.2 REST API and the OAI-PMH 2.0 endpoint both answer unauthenticated GETs. A login surface exists for deposit, workflow and administrative operations, which are not part of the public read contract catalogued here.'
kind: authentication
layout: security
method: probed
name: University Of The Witwatersrand Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of the Witwatersrand secures its APIs with none and session across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of the Witwatersrand
provider_slug: university-of-the-witwatersrand
scheme_count: 2
schemes:
- description: Public read of communities, collections, items, discovery/browse and every OAI-PMH verb requires no credential. Verified live 2026-08-30.
  evidence:
  - note: '"authenticated": false, "okay": true on an unauthenticated call'
    status: 200
    url: https://wiredspace.wits.ac.za/server/api/authn/status
  - note: paginated HAL collection returned with no credential
    status: 200
    url: https://wiredspace.wits.ac.za/server/api/core/communities
  - note: OAI-PMH Identify answered anonymously
    status: 200
    url: https://wiredspace.wits.ac.za/server/oai/request?verb=Identify
  name: Anonymous read
  type: none
- description: DSpace login/logout endpoints for authenticated deposit and administration. Not self-serve — accounts are issued through Wits institutional identity, not a developer signup.
  endpoints:
    login: https://wiredspace.wits.ac.za/server/api/authn/login
    logout: https://wiredspace.wits.ac.za/server/api/authn/logout
    status: https://wiredspace.wits.ac.za/server/api/authn/status
  evidence:
  - note: HAL document advertising login, logout and status
    status: 200
    url: https://wiredspace.wits.ac.za/server/api/authn
  name: DSpace session login
  type: session
slug: university-of-the-witwatersrand-authentication
source_filename: university-of-the-witwatersrand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live probes of https://wiredspace.wits.ac.za/server/api/authn and /authn/status\nx-operator: institution\nprovider: University of the Witwatersrand\nproviderId: university-of-the-witwatersrand\ndescription: >-\n  Authentication posture of the institution-operated WIReDSpace surfaces only. The previous version\n  of this file was derived from the Figshare v2 OAuth contract (authorizationUrl\n  https://figshare.com/account/applications/authorize, tokenUrl https://api.figshare.com/v2/token)\n  and therefore described the vendor's authorization server, not the university's — it was removed\n  on 2026-08-30 together with the vendor spec it came from. WIReDSpace read access is anonymous:\n  the DSpace 9.2 REST API and the OAI-PMH 2.0 endpoint both answer unauthenticated GETs. A login\n  surface exists for deposit, workflow and administrative operations, which are not part of the\n  public read contract catalogued here.\nsummary:\n\
  \  types:\n  - none\n  - session\n  anonymous_read: true\n  oauth2_flows: []\nschemes:\n- name: Anonymous read\n  type: none\n  description: >-\n    Public read of communities, collections, items, discovery/browse and every OAI-PMH verb requires\n    no credential. Verified live 2026-08-30.\n  evidence:\n  - url: https://wiredspace.wits.ac.za/server/api/authn/status\n    status: 200\n    note: '\"authenticated\": false, \"okay\": true on an unauthenticated call'\n  - url: https://wiredspace.wits.ac.za/server/api/core/communities\n    status: 200\n    note: paginated HAL collection returned with no credential\n  - url: https://wiredspace.wits.ac.za/server/oai/request?verb=Identify\n    status: 200\n    note: OAI-PMH Identify answered anonymously\n- name: DSpace session login\n  type: session\n  description: >-\n    DSpace login/logout endpoints for authenticated deposit and administration. Not self-serve —\n    accounts are issued through Wits institutional identity, not a developer signup.\n\
  \  endpoints:\n    login: https://wiredspace.wits.ac.za/server/api/authn/login\n    logout: https://wiredspace.wits.ac.za/server/api/authn/logout\n    status: https://wiredspace.wits.ac.za/server/api/authn/status\n  evidence:\n  - url: https://wiredspace.wits.ac.za/server/api/authn\n    status: 200\n    note: HAL document advertising login, logout and status\nnotes: >-\n  Institutional SSO for Wits staff and students runs on the university's own SimpleSAMLphp identity\n  provider registered in SAFIRE (see conformance/ and the IdentityFederation pointer in apis.yml).\n  That is a SAML 2.0 federation surface, not an API authorization server, and it does not issue\n  tokens for the WIReDSpace REST API.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/authentication/university-of-the-witwatersrand-authentication.yml
summary_line: none/session · 2 schemes
tags:
- University
- Higher Education
- Education
- Research
- South Africa
- Africa
- Institutional Repository
- Research Data
- Open Access
- Identity Federation
- OAI-PMH
- DSpace
---
