---
api_key_in: []
api_specs:
- filename: purdue-rcac-api-openapi.yml
  format: yaml
  label: Purdue RCAC API
  slug: purdue-rcac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-rcac-api-openapi.yml
- filename: purdue-hfs-dining-menus-api-openapi.yml
  format: yaml
  label: Purdue HFS Dining Menus API
  slug: purdue-hfs-dining-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-hfs-dining-menus-api-openapi.yml
auth_types: []
description: Purdue University operates no single API gateway, no developer portal and no self-service key issuance. Authentication posture differs per surface and there is no published policy tying them together. Two surfaces are fully open and keyless, one is federated behind Purdue Web Authentication, and one is an open harvesting protocol.
kind: authentication
layout: security
method: probed
name: Purdue Authentication
name_suffix: Authentication
oauth_flows: []
overview: Purdue University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Purdue University
provider_slug: purdue
scheme_count: 0
schemes: []
slug: purdue-authentication
source_filename: purdue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication Profile\nspecificationVersion: '0.1'\nprovider: Purdue University\nproviderId: purdue\nx-method: generated   # manifest authorship vocabulary (build-provenance-manifest.py)\nx-source-url: https://www.rcac.purdue.edu/api\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-30 of the four institution-operated surfaces confirmed in this profile,\n  plus the securitySchemes block of Purdue RCAC's own published OpenAPI at\n  https://www.rcac.purdue.edu/api\nx-operator: institution\ndescription: >-\n  Purdue University operates no single API gateway, no developer portal and no self-service key\n  issuance. Authentication posture differs per surface and there is no published policy tying them\n  together. Two surfaces are fully open and keyless, one is federated behind Purdue Web\n  Authentication, and one is an open harvesting protocol.\nsurfaces:\n- name: Purdue RCAC API\n  baseURL: https://www.rcac.purdue.edu/api\n\
  \  x-operator: institution\n  scheme: apiKey\n  location: header\n  parameter: api_token\n  evidence: >-\n    components.securitySchemes.api_token in the provider's own OpenAPI document\n    (type apiKey, name api_token, in header).\n  self_service: false\n  observed_behavior: >-\n    GET https://www.rcac.purdue.edu/api/groups without a token returns HTTP 500 with a\n    \"Purdue Web Authentication\" HTML login page rather than a 401 with a WWW-Authenticate\n    challenge. Probed 2026-08-30. Token issuance is not documented publicly; it appears to be\n    tied to Purdue institutional identity.\n  notes: >-\n    The contract is public and complete; the endpoints are not. This is auth_required, not\n    undocumented - the two are different findings and only the second is a gap in publishing.\n- name: Purdue HFS Dining Menus API\n  baseURL: https://api.hfs.purdue.edu/menus/v2\n  x-operator: institution\n  scheme: none\n  self_service: true\n  observed_behavior: >-\n    GET /menus/v2/locations\
  \ returned 200 with a 35,766-byte JSON body with no credential of any\n    kind. No key, quota, sign-up or terms page was found. Probed 2026-08-30.\n- name: PURR OAI-PMH\n  baseURL: https://purr.purdue.edu/oaipmh\n  x-operator: institution\n  scheme: none\n  self_service: true\n  observed_behavior: >-\n    verb=Identify and verb=ListSets both returned 200 with valid OAI-PMH 2.0 XML, keyless.\n    Probed 2026-08-30.\n- name: Purdue Shibboleth Identity Provider\n  baseURL: https://sso.purdue.edu/idp\n  x-operator: institution\n  scheme: saml2\n  self_service: false\n  observed_behavior: >-\n    SAML 2.0 IdP metadata is served publicly and unauthenticated at\n    https://sso.purdue.edu/idp/shibboleth and signed from InCommon MDQ. The IdP itself\n    authenticates Purdue accounts and is reachable to relying parties registered in InCommon or\n    eduGAIN; it is not open to arbitrary service providers.\n  entityID: https://idp.purdue.edu/idp/shibboleth\ngaps:\n- No published authentication documentation\
  \ for the HFS menus API.\n- No self-service credential issuance for any Purdue-operated API.\n- RCAC returns 500 and an HTML login page where a 401 and a JSON error body belong.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/authentication/purdue-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Indiana
- Public Research University
- Land-Grant University
- Association of American Universities
- Big Ten Academic Alliance
- Research Computing
- Research Repository
- Identity Federation
- OAI-PMH
- Campus Life
- Course Catalog
---
