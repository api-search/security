---
api_key_in: []
api_specs:
- filename: university-of-edinburgh-elm-api-openapi.yml
  format: yaml
  label: ELM — Edinburgh Language Models API
  slug: elm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-elm-api-openapi.yml
- filename: university-of-edinburgh-catalogue-api-openapi.yml
  format: yaml
  label: University of Edinburgh Catalogue API
  slug: university-of-edinburgh-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-catalogue-api-openapi.yml
- filename: university-of-edinburgh-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Edinburgh OAI PMH API
  slug: university-of-edinburgh-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-oai-pmh-api-openapi.yml
- filename: university-of-edinburgh-repository-api-openapi.yml
  format: yaml
  label: University of Edinburgh Repository API
  slug: university-of-edinburgh-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-repository-api-openapi.yml
auth_types: []
description: How authentication works across the institution-operated University of Edinburgh surfaces. Every statement below was observed by probing on 2026-08-19.
kind: authentication
layout: security
method: probed
name: University Of Edinburgh Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Edinburgh declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Edinburgh
provider_slug: university-of-edinburgh
scheme_count: 0
schemes: []
slug: university-of-edinburgh-authentication
source_filename: university-of-edinburgh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: University of Edinburgh — Authentication\ndescription: >-\n  How authentication works across the institution-operated University of Edinburgh\n  surfaces. Every statement below was observed by probing on 2026-08-19.\ngenerated: '2026-08-19'\nmethod: probed\nsource: https://datashare.ed.ac.uk/server/api/authn\n\nsurfaces:\n\n- surface: Edinburgh DataShare REST API\n  operator: institution\n  baseURL: https://datashare.ed.ac.uk/server/api\n  anonymous_access: partial\n  detail: >-\n    Anonymous callers can read /core/communities, /core/collections,\n    /discover/search/objects and /discover/browses. /core/items and\n    /core/bitstreams return 401 to anonymous callers on this deployment, which is\n    stricter than a stock DSpace 8 install. Authenticated access uses DSpace's own\n    /authn endpoints, which on this deployment federate to the University's\n    Shibboleth IdP; there is no self-service API key or OAuth client registration.\n  evidence:\n  - url: https://datashare.ed.ac.uk/server/api/core/communities?size=1\n\
  \    status: 200\n  - url: https://datashare.ed.ac.uk/server/api/core/items?size=1\n    status: 401\n  - url: https://datashare.ed.ac.uk/server/api/core/bitstreams?size=1\n    status: 401\n\n- surface: Edinburgh Research Archive (ERA) REST API\n  operator: institution\n  baseURL: https://era.ed.ac.uk/server/api\n  anonymous_access: partial\n  detail: Same posture as DataShare — communities, collections and browse read anonymously, items 401.\n  evidence:\n  - url: https://era.ed.ac.uk/server/api/core/communities?size=1\n    status: 200\n  - url: https://era.ed.ac.uk/server/api/core/items?size=1\n    status: 401\n  - url: https://era.ed.ac.uk/server/api/discover/browses\n    status: 200\n\n- surface: OAI-PMH endpoints (DataShare, ERA)\n  operator: institution\n  anonymous_access: full\n  detail: >-\n    Fully anonymous. No key, no registration, no rate-limit header observed. This is\n    the most open machine-readable surface the institution operates and the one a\n    harvester should\
  \ use.\n  evidence:\n  - url: https://datashare.ed.ac.uk/oai/request?verb=Identify\n    status: 200\n  - url: https://era.ed.ac.uk/oai/request?verb=Identify\n    status: 200\n\n- surface: EIDF Data Catalogue (CKAN)\n  operator: institution\n  baseURL: https://catalogue.eidf.ac.uk/api/3/action\n  anonymous_access: full\n  detail: >-\n    Read actions require no API key. The deployment carries a custom `eidf_oidc_auth`\n    CKAN extension, so authenticated write access is OIDC-based and tied to EIDF\n    project accounts rather than to a public developer signup.\n  evidence:\n  - url: https://catalogue.eidf.ac.uk/api/3/action/status_show\n    status: 200\n    observed: 'extensions include eidf_oidc_auth'\n  - url: https://catalogue.eidf.ac.uk/api/3/action/package_search?rows=1\n    status: 200\n\n- surface: Enterprise API gateway\n  operator: institution\n  baseURL: https://api.ed.ac.uk\n  anonymous_access: none\n  detail: >-\n    api.ed.ac.uk is live and resolves to a WSO2 Choreo tenant\
  \ named `uoe`\n    (f5aad5f4-...-prod.prod.uoe.choreoapis.dev via an eu-west-2 ELB). Every path\n    probed returned the gateway's own JSON 404 envelope, including /openapi,\n    /api-docs, /services and /.well-known/openid-configuration. The gateway exists\n    and is Edinburgh-operated, but no route, catalogue or developer portal is\n    exposed to unauthenticated callers. This is a gated surface, not an absent one.\n  evidence:\n  - url: https://api.ed.ac.uk/\n    status: 404\n    observed: '{\"message\":\"Not Found\",\"description\":\"The requested resource is not available.\",\"code\":\"404\"}'\n  - url: https://api.ed.ac.uk/openapi\n    status: 404\n  - url: https://api.ed.ac.uk/.well-known/openid-configuration\n    status: 404\n\nidentity_federation:\n  operator: institution\n  entityID: https://idp.ed.ac.uk/shibboleth\n  metadata: https://idp.ed.ac.uk/idp/shibboleth\n  detail: >-\n    Shibboleth IdP, SAML 2.0 metadata published unauthenticated. Note that the IdP\n    web root (https://idp.ed.ac.uk/)\
  \ returns 403 by design — the metadata path is the\n    machine-readable surface and it answers 200.\n  evidence:\n  - url: https://idp.ed.ac.uk/idp/shibboleth\n    status: 200\n  - url: https://idp.ed.ac.uk/\n    status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/authentication/university-of-edinburgh-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Scotland
- Russell Group
- Research Repository
- Open Data
- Identity Federation
- Research Computing
- OAI-PMH
- Artificial Intelligence
---
