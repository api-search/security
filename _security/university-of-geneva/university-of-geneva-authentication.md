---
api_key_in: []
api_specs:
- filename: university-of-geneva-access-api-openapi.yml
  format: yaml
  label: Yareta Access API
  slug: university-of-geneva-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/openapi/university-of-geneva-access-api-openapi.yml
- filename: university-of-geneva-ingest-api-openapi.yml
  format: yaml
  label: Yareta Ingest API
  slug: university-of-geneva-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/openapi/university-of-geneva-ingest-api-openapi.yml
- filename: university-of-geneva-oai-pmh-api-openapi.yml
  format: yaml
  label: Yareta OAI-PMH Provider API
  slug: university-of-geneva-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/openapi/university-of-geneva-oai-pmh-api-openapi.yml
auth_types: []
description: How the University of Geneva's institution-operated surfaces authenticate. There is no single institutional API gateway, no developer key issuance, and no self-service credential flow of any kind — UNIGE's programmable surfaces are either fully anonymous (open-science harvesting) or gated behind the university's own SWITCH edu-ID / SWITCHaai (Shibboleth SAML 2.0) identity, which is available to affiliates and federation partners rather than to the public.
kind: authentication
layout: security
method: probed
name: University Of Geneva Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Geneva declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Geneva
provider_slug: university-of-geneva
scheme_count: 0
schemes: []
slug: university-of-geneva-authentication
source_filename: university-of-geneva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: University of Geneva\nproviderId: university-of-geneva\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live HTTP probes of every institution-operated University of Geneva surface on 2026-09-01,\n  plus the SWITCHaai federation metadata document. Nothing here is inferred from documentation\n  prose; each entry names the response that produced it.\ndescription: >-\n  How the University of Geneva's institution-operated surfaces authenticate. There is no single\n  institutional API gateway, no developer key issuance, and no self-service credential flow of\n  any kind — UNIGE's programmable surfaces are either fully anonymous (open-science harvesting)\n  or gated behind the university's own SWITCH edu-ID / SWITCHaai (Shibboleth SAML 2.0) identity,\n  which is available to affiliates and federation partners rather than to the public.\n\nsurfaces:\n- name: Archive ouverte UNIGE OAI-PMH\n  host:\
  \ archive-ouverte.unige.ch\n  x-operator: institution\n  scheme: none\n  anonymous: true\n  detail: >-\n    Anonymous. verb=Identify, verb=ListMetadataFormats and verb=ListSets all return 200 with\n    no credential. No API key, no registration, no rate-limit challenge observed.\n  evidence:\n  - url: https://archive-ouverte.unige.ch/oai?verb=Identify\n    status: 200\n    probed: '2026-09-01'\n\n- name: Yareta access module\n  host: access.yareta.unige.ch\n  x-operator: institution\n  scheme: http-bearer\n  anonymous: partial\n  detail: >-\n    Bearer token. Protected operations answer an unauthenticated request with HTTP 401 and\n    `WWW-Authenticate: Bearer` and an empty body. One endpoint is genuinely public and\n    unauthenticated: GET /default-configuration returns 200 application/json (13.3 KB) and\n    exposes the deployment's ORCID OAuth wiring, OAI-PMH settings, Shibboleth header handling\n    and the institution's ROR id. GET /current-configuration is 401.\n    The machine-readable\
  \ contract itself is gated: /v3/api-docs and\n    /v3/api-docs/swagger-config both return 401, while the Swagger UI shell at\n    /swagger-ui/index.html returns 200 and therefore renders nothing to an anonymous reader.\n  evidence:\n  - url: https://access.yareta.unige.ch/access/deposits\n    status: 401\n    header: 'www-authenticate: Bearer'\n    probed: '2026-09-01'\n  - url: https://access.yareta.unige.ch/default-configuration\n    status: 200\n    probed: '2026-09-01'\n  - url: https://access.yareta.unige.ch/v3/api-docs\n    status: 401\n    probed: '2026-09-01'\n  - url: https://access.yareta.unige.ch/swagger-ui/index.html\n    status: 200\n    detail: 734-byte Swagger UI shell; the definition it would load is 401.\n    probed: '2026-09-01'\n\n- name: Yareta ingest module\n  host: ingest.yareta.unige.ch\n  x-operator: institution\n  scheme: http-bearer\n  anonymous: false\n  detail: Same bearer scheme as the access module; the contract endpoint is gated identically.\n  evidence:\n\
  \  - url: https://ingest.yareta.unige.ch/v3/api-docs\n    status: 401\n    probed: '2026-09-01'\n  - url: https://ingest.yareta.unige.ch/swagger-ui/index.html\n    status: 200\n    probed: '2026-09-01'\n\n- name: UNIGE GitLab REST API v4\n  host: gitlab.unige.ch\n  x-operator: institution\n  scheme: none\n  anonymous: partial\n  detail: >-\n    Anonymous read of public projects works. GET /api/v4/projects returns 200 with\n    X-Total 1146 and no credential. Instance-wide endpoints require a token:\n    GET /api/v4/version returns 401. Personal access tokens are issued only to affiliates,\n    who sign in through the university's Shibboleth SP (entityID\n    https://gitlab.unige.ch/shibboleth in SWITCHaai).\n  evidence:\n  - url: https://gitlab.unige.ch/api/v4/projects?per_page=1\n    status: 200\n    detail: 'X-Total: 1146'\n    probed: '2026-09-01'\n  - url: https://gitlab.unige.ch/api/v4/version\n    status: 401\n    probed: '2026-09-01'\n\n- name: Terminus protein-prediction API\n\
  \  host: terminus.unige.ch\n  x-operator: institution\n  scheme: none\n  anonymous: true\n  detail: >-\n    Anonymous HTTP POST to http://terminus.unige.ch/query/<predictor>/<format>. No credential,\n    no registration, no quota published. Documentation page returns 200.\n  evidence:\n  - url: https://terminus.unige.ch/info/API\n    status: 200\n    probed: '2026-09-01'\n\nfederated_identity:\n  provider: SWITCH edu-ID / SWITCHaai\n  entity_id: https://idp.unige.ch/idp/shibboleth\n  protocol: SAML 2.0\n  scope: unige.ch\n  sso:\n  - https://unige.login.eduid.ch/idp/profile/SAML2/Redirect/SSO\n  - https://unige.login.eduid.ch/idp/profile/SAML2/POST/SSO\n  detail: >-\n    The institution's own Shibboleth IdP, registered in the Swiss national research and\n    education federation. This is the credential behind essentially every gated UNIGE surface,\n    including Yareta, GitLab, Moodle, the Archive ouverte deposit interface and the swisscovery\n    library account. 123 unige.ch service-provider\
  \ and identity-provider entities are registered\n    in the same federation metadata document.\n  evidence:\n  - url: https://metadata.aai.switch.ch/metadata.switchaai.xml\n    status: 200\n    probed: '2026-09-01'\n\ngaps:\n- No OAuth 2.0 / OpenID Connect authorization-server metadata is published at any UNIGE host.\n- No RFC 9728 protected-resource metadata and no /.well-known catalog on any probed host.\n- No public developer key issuance, no self-service onboarding, no sandbox credential.\n- The Yareta OpenAPI is behind the same bearer gate as the API, so an unauthenticated agent\n  cannot obtain the contract from the origin; the copy in openapi/ is a derived conversion.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/authentication/university-of-geneva-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Public Research University
- Open Science
- Research Data
- Institutional Repository
- Research Repository
- Identity Federation
- OAI-PMH
- Switzerland
- Europe
---
