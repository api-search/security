---
api_key_in: []
api_specs:
- filename: university-of-ottawa-ruor-dspace-rest-openapi.yml
  format: yaml
  label: uO Research DSpace REST API
  slug: ruor-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-ottawa/refs/heads/main/openapi/university-of-ottawa-ruor-dspace-rest-openapi.yml
- filename: university-of-ottawa-ruor-oai-pmh-openapi.yml
  format: yaml
  label: uO Research OAI-PMH
  slug: ruor-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-ottawa/refs/heads/main/openapi/university-of-ottawa-ruor-oai-pmh-openapi.yml
- filename: university-of-ottawa-www-drupal-jsonapi-openapi.yml
  format: yaml
  label: uottawa.ca Content JSON:API
  slug: www-jsonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-ottawa/refs/heads/main/openapi/university-of-ottawa-www-drupal-jsonapi-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Ottawa Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Ottawa declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Ottawa
provider_slug: university-of-ottawa
scheme_count: 0
schemes: []
slug: university-of-ottawa-authentication
source_filename: university-of-ottawa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://ruor.uottawa.ca/server/api/authn/status\nx-operator: institution\nnote: >-\n  How authentication actually behaves on the University of Ottawa's institution-operated\n  surfaces, established by live anonymous requests on 2026-09-01. uOttawa publishes no\n  developer documentation for any of these, so every statement below is a probe result.\nsurfaces:\n  - id: ruor-dspace-rest\n    name: uO Research DSpace REST API\n    base_url: https://ruor.uottawa.ca/server/api\n    operator: institution\n    public_read: partial\n    scheme: none_required_for_public_reads\n    evidence: >-\n      GET /authn/status returns HTTP 200 with {\"okay\": true, \"authenticated\": false,\n      \"authenticationMethod\": null}, confirming anonymous calls are accepted. GET\n      /core/communities and /core/collections return 200 anonymously; GET /core/items and\n      GET /core/bitstreams/{uuid} return 401, so item and bitstream enumeration is\
  \ closed to\n      anonymous callers and public discovery must go through /discover/search/objects.\n    write_access: >-\n      Not attempted. DSpace 8 supports session-based login at /api/authn/login plus an\n      X-XSRF-TOKEN CSRF flow; no credentials were used and no write path was probed.\n  - id: ruor-oai-pmh\n    name: uO Research OAI-PMH\n    base_url: https://ruor.uottawa.ca/server/oai/request\n    operator: institution\n    public_read: true\n    scheme: none\n    evidence: >-\n      Identify, ListMetadataFormats, ListSets and ListRecords all returned HTTP 200 with no\n      credentials, key, or referrer requirement.\n  - id: www-jsonapi\n    name: uottawa.ca Content JSON:API\n    base_url: https://www.uottawa.ca/en/jsonapi\n    operator: institution\n    public_read: true\n    scheme: none\n    evidence: >-\n      The resource index, node/article, node/alert and taxonomy_term/tags all returned HTTP\n      200 anonymously. Drupal's JSON:API module is running read-only for anonymous\
  \ users;\n      no write was attempted.\n  - id: caf-idp\n    name: uOttawa Shibboleth Identity Provider\n    base_url: https://fca-caf.uottawa.ca/idp\n    operator: institution\n    public_read: true\n    scheme: saml2\n    evidence: >-\n      The SAML 2.0 metadata document at /idp/shibboleth is served anonymously (HTTP 200). The\n      IdP itself authenticates uottawa.ca principals for federated services; this profile\n      records only the public metadata endpoint.\nnegative_probes:\n  - url: https://www.uottawa.ca/.well-known/openid-configuration\n    status: 404\n    note: No OIDC discovery document on the primary web property.\n  - url: https://www.uottawa.ca/.well-known/security.txt\n    status: 404\n    note: No RFC 9116 security contact.\n  - url: https://api.uottawa.ca/\n    status: 0\n    note: Host does not resolve. No central API gateway.\n  - url: https://developer.uottawa.ca/\n    status: 0\n    note: Host does not resolve. No developer portal, so no key-issuing or onboarding\
  \ flow exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-ottawa/refs/heads/main/authentication/university-of-ottawa-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Canada
- Ontario
- Bilingual
- Public Research University
- U15
- Institutional Repository
- Research Data
- Library
- Course Catalog
- Identity Federation
- Shibboleth
- SAML
- DSpace
- OAI-PMH
- JSON API
- Open Access
- DataCite
- Crossref
- ROR
---
