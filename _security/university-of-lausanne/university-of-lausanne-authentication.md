---
api_key_in: []
api_specs:
- filename: university-of-lausanne-projects-json-api-openapi.yml
  format: yaml
  label: SPICA Atlas Projects.json API
  slug: university-of-lausanne-projects-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-projects-json-api-openapi.yml
- filename: university-of-lausanne-projects-api-openapi.yml
  format: yaml
  label: SPICA Atlas Projects API
  slug: university-of-lausanne-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-projects-api-openapi.yml
- filename: university-of-lausanne-core-api-openapi.yml
  format: yaml
  label: IRIS Repository Core API (DSpace REST)
  slug: university-of-lausanne-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-core-api-openapi.yml
- filename: university-of-lausanne-discover-api-openapi.yml
  format: yaml
  label: IRIS Repository Discover API (DSpace Discovery)
  slug: university-of-lausanne-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-discover-api-openapi.yml
- filename: university-of-lausanne-iris-repository-dspace-rest-api-api-openapi.yml
  format: yaml
  label: IRIS Repository API root (DSpace REST)
  slug: university-of-lausanne-iris-repository-dspace-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-iris-repository-dspace-rest-api-api-openapi.yml
- filename: university-of-lausanne-oai-pmh-api-openapi.yml
  format: yaml
  label: IRIS OAI-PMH
  slug: university-of-lausanne-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-oai-pmh-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Lausanne Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Lausanne declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Lausanne
provider_slug: university-of-lausanne
scheme_count: 0
schemes: []
slug: university-of-lausanne-authentication
source_filename: university-of-lausanne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of api.unil.ch, spica.unil.ch, my.unil.ch and the\n  SWITCHaai federation metadata. Written by API Evangelist, not published by the\n  University of Lausanne.\nnote: >-\n  UNIL publishes no developer portal, no API key programme and no client\n  registration of any kind. Every anonymously callable surface below is open\n  read; everything else is behind institutional SSO that only a UNIL account\n  holder or a SWITCHaai/eduGAIN home organisation can traverse. There is no\n  third-party developer path onto any UNIL API.\nsurfaces:\n- name: SPICA Atlas API\n  host: spica.unil.ch\n  scheme: none\n  detail: >-\n    Anonymous open read. /projects.json and /projects/query.json both returned\n    200 with no credential on 2026-09-01. No key, no quota header, no\n    registration.\n- name: IRIS DSpace REST API\n  host: api.unil.ch\n  scheme: mixed\n  detail: >-\n    Anonymous open read for /core/communities,\
  \ /core/collections and\n    /discover/search/objects (all 200 on 2026-09-01). /core/items and\n    /core/bitstreams return 401 to an anonymous client. Authenticated access\n    uses the DSpace 7 /api/authn contract (JWT bearer issued after login,\n    CSRF token via DSPACE-XSRF-TOKEN), reachable in the root document's HAL\n    _links as `authn` and `authorizations`, but IRIS is behind UNIL SSO and\n    there is no self-service account.\n- name: IRIS OAI-PMH\n  host: api.unil.ch\n  scheme: none\n  detail: >-\n    Anonymous open harvest on both contexts, /oai/request and\n    /oai/openairecris. No credential, no registration, no rate-limit header\n    observed.\n- name: UNIL Shibboleth Identity Provider\n  host: aai.unil.ch (entityID namespace; no public A record) / unil.login.eduid.ch\n  scheme: saml2-shibboleth\n  detail: >-\n    entityID https://aai.unil.ch/idp/shibboleth, an IDPSSODescriptor with\n    OrganizationName unil.ch and shibmd:Scope unil.ch, registered in SWITCHaai\n    and\
  \ exported to eduGAIN. This is the credential authority for everything\n    behind my.unil.ch and for the 145 unil.ch entities registered in the same\n    federation. Its SSO endpoints run on SWITCH's edu-ID platform at\n    unil.login.eduid.ch, so UNIL owns the entity, the scope and the identities\n    while SWITCH hosts the endpoint. The SAML metadata is anonymously readable\n    only from SWITCH's published aggregates\n    (metadata.aai.switch.ch/metadata.switchaai+idp.xml); SWITCH exposes no\n    per-entity MDQ service — /entities/<entityID> answers 400 and\n    /mdq/entities/<entityID> 302s to an HTML help page. Authentication itself\n    is available only to federation members.\n- name: my.unil.ch\n  host: my.unil.ch\n  scheme: institutional-sso\n  detail: >-\n    The gateway in front of UNIL's student-information, timetable and\n    administrative services. Returned 200 (a login surface) on 2026-09-01.\n    Nothing behind it is documented as an API and nothing is reachable without\n\
  \    a UNIL identity.\n- name: ADFS / STS\n  host: sts.unil.ch\n  scheme: ws-federation\n  detail: >-\n    A second UNIL federation entity, http://sts.unil.ch/adfs/services/trust,\n    registered in SWITCHaai alongside the Shibboleth IdP.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/authentication/university-of-lausanne-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Switzerland
- Open Science
- Research Data
- Institutional Repository
- Research Repository
- Identity Federation
- OAI-PMH
- Course Catalog
- Research Computing
---
