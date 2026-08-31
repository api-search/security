---
api_key_in: []
api_specs:
- filename: ubc-access-api-openapi.yml
  format: yaml
  label: UBC Library Abacus Dataverse API
  slug: abacus-dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubc/refs/heads/main/openapi/ubc-access-api-openapi.yml
- filename: ubc-collections-api-openapi.yml
  format: yaml
  label: University of British Columbia Collections API
  slug: ubc-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubc/refs/heads/main/openapi/ubc-collections-api-openapi.yml
auth_types: []
description: 'How authentication actually works across UBC''s institution-operated programmable surfaces. UBC has no single developer identity: each surface authenticates on its own terms, and the enterprise gateway is not self-service at all.'
kind: authentication
layout: security
method: probed
name: Ubc Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of British Columbia declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of British Columbia
provider_slug: ubc
scheme_count: 0
schemes: []
slug: ubc-authentication
source_filename: ubc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: University of British Columbia\nproviderId: ubc\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes of oc-index.library.ubc.ca, abacus.library.ubc.ca, authentication.ubc.ca and\n  api.ubc.ca on 2026-08-19; UBC Library's own documentation source at\n  github.com/ubc-library/docs-open-collections-api (data/api.twig.html); and\n  openapi/_original/ubc-abacus-dataverse.yaml.\ndescription: >-\n  How authentication actually works across UBC's institution-operated programmable surfaces.\n  UBC has no single developer identity: each surface authenticates on its own terms, and the\n  enterprise gateway is not self-service at all.\n\nsurfaces:\n- id: ubc:open-collections\n  name: UBC Library Open Collections API\n  x-operator: institution\n  type: apiKey\n  in: query\n  parameterName: apiKey\n  anonymousAccess: true\n  detail: >-\n    Reads work with no credential at a shared ceiling\
  \ of 10 requests per minute per IP. UBC\n    Library issues a personal key on email registration, raising the ceiling to 200 requests\n    per minute. There is no OAuth, no client registration and no token endpoint.\n  registration: https://open.library.ubc.ca/docs\n  evidence:\n  - url: https://oc-index.library.ubc.ca/collections\n    status: 200\n    detail: Returned 362 collections with no credential supplied.\n  - url: https://oc-index.library.ubc.ca/collections/berkpost/items?limit=2\n    status: 429\n    detail: >-\n      \"Too Many Requests from IP 141.157.211.19 (max 10 per minute, tried 10). Expires in 12\n      seconds\" — the anonymous ceiling enforced live.\n\n- id: ubc:abacus-dataverse\n  name: UBC Library Abacus Dataverse API\n  x-operator: institution\n  type: apiKey\n  in: header\n  parameterName: X-Dataverse-key\n  alternateParameter: key (query string)\n  anonymousAccess: true\n  detail: >-\n    Dataverse's standard model. Read operations against public dataverses, datasets\
  \ and files\n    are open; every write operation and every admin operation requires an API token issued\n    from a signed-in Abacus account. Accounts are created by UBC Library / Abacus support.\n  evidence:\n  - url: https://abacus.library.ubc.ca/api/info/version\n    status: 200\n    detail: '{\"status\":\"OK\",\"data\":{\"version\":\"5.9\",\"build\":null}} returned unauthenticated.'\n  - url: openapi/_original/ubc-abacus-dataverse.yaml\n    status: 200\n    detail: Contract exposes a `key` query parameter on access operations.\n\n- id: ubc:abacus-oai-pmh\n  name: Abacus OAI-PMH\n  x-operator: institution\n  type: none\n  anonymousAccess: true\n  detail: >-\n    Unauthenticated by protocol. Public visibility is controlled by set membership rather than\n    credential — the abacus_open set is described as \"Datasets available for the public without\n    authentication\", while sfulicensed and peer sets are not.\n  evidence:\n  - url: https://abacus.library.ubc.ca/oai?verb=Identify\n\
  \    status: 200\n\n- id: ubc:shibboleth-idp\n  name: UBC Shibboleth Identity Provider\n  x-operator: institution\n  type: saml2\n  anonymousAccess: false\n  detail: >-\n    UBC's own SAML 2.0 identity provider, entityID https://authentication.ubc.ca, asserting the\n    ubc.ca scope. This is the credential surface that every other UBC service federates\n    against, and it is the one machine-readable artifact UBC publishes about its own identity\n    layer. Signing certificate is self-issued to CN=authentication.ubc.ca.\n  evidence:\n  - url: https://authentication.ubc.ca/idp/shibboleth\n    status: 200\n    detail: 9,213 bytes application/xml SAML metadata, served without credential.\n\n- id: ubc:iec-api-gateway\n  name: UBC Integration Enablement Centre API gateway\n  x-operator: institution\n  type: gated\n  anonymousAccess: false\n  detail: >-\n    api.ubc.ca is live and refuses everything. There is no public token endpoint, no client\n    registration and no published scheme. Access\
  \ is granted per-API through UBC's Data Access\n    Framework, requested by ServiceNow ticket, and the API list itself sits behind UBC's\n    Confluence login. The authentication story is an internal procurement process, not an\n    interface.\n  registration: https://ubc.service-now.com/selfservice\n  evidence:\n  - url: https://api.ubc.ca/\n    status: 403\n    detail: >-\n      nginx 403 Forbidden with HSTS. DNS resolves api.ubc.ca -> api.iec.it.ubc.ca ->\n      ubc-iec.lb.anypointdns.net (MuleSoft Anypoint load balancer).\n  - url: https://confluence.it.ubc.ca/x/Jo14Bw\n    status: 200\n    detail: >-\n      The IEC's own API list. Redirects to confluence.it.ubc.ca/my.logout.php3?errorcode=19 —\n      authentication required, contents not readable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubc/refs/heads/main/authentication/ubc-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Public Research University
- Canada
- British Columbia
- U15
- Library
- Digital Collections
- Research Data
- Research Repository
- Open Data
- Identity Federation
- OAI-PMH
- IIIF
- Dataverse
---
