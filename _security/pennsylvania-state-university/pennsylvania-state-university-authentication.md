---
api_key_in: []
api_specs:
- filename: pennsylvania-state-university-researcher-metadata-api-openapi.yml
  format: yaml
  label: Researcher Metadata Database (RMD) API
  slug: rmd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-researcher-metadata-api-openapi.yml
- filename: pennsylvania-state-university-scholarsphere-api-openapi.yml
  format: yaml
  label: ScholarSphere API
  slug: scholarsphere
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-scholarsphere-api-openapi.yml
- filename: pennsylvania-state-university-buildings-api-openapi.yml
  format: yaml
  label: Pennsylvania State University Buildings API
  slug: pennsylvania-state-university-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-buildings-api-openapi.yml
- filename: pennsylvania-state-university-campuses-api-openapi.yml
  format: yaml
  label: Pennsylvania State University Campuses API
  slug: pennsylvania-state-university-campuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-campuses-api-openapi.yml
- filename: pennsylvania-state-university-events-api-openapi.yml
  format: yaml
  label: Pennsylvania State University Events API
  slug: pennsylvania-state-university-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-events-api-openapi.yml
- filename: pennsylvania-state-university-health-api-openapi.yml
  format: yaml
  label: Pennsylvania State University Health API
  slug: pennsylvania-state-university-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-health-api-openapi.yml
- filename: pennsylvania-state-university-rooms-api-openapi.yml
  format: yaml
  label: Pennsylvania State University Rooms API
  slug: pennsylvania-state-university-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-rooms-api-openapi.yml
auth_types:
- apiKey
- none
- saml
description: ''
kind: authentication
layout: security
method: generated
name: Pennsylvania State University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pennsylvania State University secures its APIs with apiKey, none, and saml across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pennsylvania State University
provider_slug: pennsylvania-state-university
scheme_count: 5
schemes:
- api: Researcher Metadata Database (RMD) API
  description: License key issued by Penn State University Libraries. Requested through https://metadata.libraries.psu.edu/ — not self-service.
  in: header
  name: rmd-api-key
  parameter: X-API-Key
  sources:
  - openapi/pennsylvania-state-university-researcher-metadata-api-openapi.yml
  - examples/pennsylvania-state-university-rmd-unauthenticated-example.json
  type: apiKey
  verified: 'GET https://metadata.libraries.psu.edu/v1/organizations without the header returns 401 application/json {"message":"401: Request not authorized. Please provide a valid API key for access.","code":401} (probed 2026-08-30).'
  x-operator: institution
- api: ScholarSphere API
  description: Key obtained from the ScholarSphere team at Penn State University Libraries; the spec states it is included in the header of all requests. Note the underscore form of the header name — it is X_API_KEY, not X-API-Key, and differs from the sibling RMD service.
  in: header
  name: scholarsphere-api-key
  parameter: X_API_KEY
  sources:
  - openapi/pennsylvania-state-university-scholarsphere-api-openapi.yml
  - examples/pennsylvania-state-university-scholarsphere-unauthenticated-example.json
  type: apiKey
  verified: GET https://scholarsphere.psu.edu/api/v1/dois without the header returns 401 application/json (probed 2026-08-30).
  x-operator: institution
- api: LionSpaceFIS Facilities API
  description: No authentication. The Office of Physical Plant facilities API answers unauthenticated GETs.
  name: lionspacefis-open
  sources:
  - examples/pennsylvania-state-university-listCampuses-example.json
  type: none
  verified: GET https://apps.opp.psu.edu/fis-api/v1/campuses returns 200 application/json and /fis-api/health returns 200 with appStatus UP, both with no credential (probed 2026-08-30).
  x-operator: institution
- api: ETDA OAI-PMH provider
  description: OAI-PMH is an open harvesting protocol; no credential, no registration.
  name: etda-oai-open
  type: none
  verified: GET https://etda.libraries.psu.edu/catalog/oai?verb=Identify returns 200 text/xml (probed 2026-08-30).
  x-operator: institution
- api: Penn State Identity Federation (InCommon)
  description: Institutional SSO, not an API credential. entityID urn:mace:incommon:psu.edu; IdP at as1.fim.psu.edu speaking Shibboleth 1.0, SAML 1.1 and SAML 2.0. This is what stands in front of every internal Penn State service and is the reason most of the institution's REST surface is unreadable from outside.
  name: incommon-shibboleth-idp
  type: saml
  verified: https://as1.fim.psu.edu/idp/shibboleth returns 200 application/xml (9,398 bytes) directly from Penn State, and https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Apsu.edu returns 200 application/samlmetadata+xml from the federation (both probed 2026-08-30).
  x-operator: institution
slug: pennsylvania-state-university-authentication
source_filename: pennsylvania-state-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: generated\nx-evidence: probed\nsource: >-\n  openapi/pennsylvania-state-university-researcher-metadata-api-openapi.yml,\n  openapi/pennsylvania-state-university-scholarsphere-api-openapi.yml,\n  openapi/pennsylvania-state-university-fis-* (LionSpaceFIS), plus live 401/200 probes 2026-08-30.\nnote: >-\n  Penn State has no single API gateway and no unified credential. Each institution-operated surface\n  issues its own key out of the unit that runs it, and the campus-wide identity layer (Shibboleth /\n  WebAccess) is not an API credential at all — it gates people, not machines. The former central\n  developer portal at docs.developer.psu.edu, which brokered elevated access to internal REST\n  services, now 302s to sites.psu.edu and no longer exists.\nsummary:\n  types:\n  - apiKey\n  - none\n  - saml\nschemes:\n- name: rmd-api-key\n  api: Researcher Metadata Database (RMD) API\n  x-operator: institution\n  type: apiKey\n  in: header\n  parameter:\
  \ X-API-Key\n  description: >-\n    License key issued by Penn State University Libraries. Requested through\n    https://metadata.libraries.psu.edu/ — not self-service.\n  verified: >-\n    GET https://metadata.libraries.psu.edu/v1/organizations without the header returns 401\n    application/json {\"message\":\"401: Request not authorized. Please provide a valid API key for\n    access.\",\"code\":401} (probed 2026-08-30).\n  sources:\n  - openapi/pennsylvania-state-university-researcher-metadata-api-openapi.yml\n  - examples/pennsylvania-state-university-rmd-unauthenticated-example.json\n- name: scholarsphere-api-key\n  api: ScholarSphere API\n  x-operator: institution\n  type: apiKey\n  in: header\n  parameter: X_API_KEY\n  description: >-\n    Key obtained from the ScholarSphere team at Penn State University Libraries; the spec states it\n    is included in the header of all requests. Note the underscore form of the header name — it is\n    X_API_KEY, not X-API-Key, and differs from\
  \ the sibling RMD service.\n  verified: >-\n    GET https://scholarsphere.psu.edu/api/v1/dois without the header returns 401 application/json\n    (probed 2026-08-30).\n  sources:\n  - openapi/pennsylvania-state-university-scholarsphere-api-openapi.yml\n  - examples/pennsylvania-state-university-scholarsphere-unauthenticated-example.json\n- name: lionspacefis-open\n  api: LionSpaceFIS Facilities API\n  x-operator: institution\n  type: none\n  description: >-\n    No authentication. The Office of Physical Plant facilities API answers unauthenticated GETs.\n  verified: >-\n    GET https://apps.opp.psu.edu/fis-api/v1/campuses returns 200 application/json and\n    /fis-api/health returns 200 with appStatus UP, both with no credential (probed 2026-08-30).\n  sources:\n  - examples/pennsylvania-state-university-listCampuses-example.json\n- name: etda-oai-open\n  api: ETDA OAI-PMH provider\n  x-operator: institution\n  type: none\n  description: >-\n    OAI-PMH is an open harvesting protocol;\
  \ no credential, no registration.\n  verified: >-\n    GET https://etda.libraries.psu.edu/catalog/oai?verb=Identify returns 200 text/xml\n    (probed 2026-08-30).\n- name: incommon-shibboleth-idp\n  api: Penn State Identity Federation (InCommon)\n  x-operator: institution\n  type: saml\n  description: >-\n    Institutional SSO, not an API credential. entityID urn:mace:incommon:psu.edu; IdP at\n    as1.fim.psu.edu speaking Shibboleth 1.0, SAML 1.1 and SAML 2.0. This is what stands in front of\n    every internal Penn State service and is the reason most of the institution's REST surface is\n    unreadable from outside.\n  verified: >-\n    https://as1.fim.psu.edu/idp/shibboleth returns 200 application/xml (9,398 bytes) directly from\n    Penn State, and https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Apsu.edu returns 200\n    application/samlmetadata+xml from the federation (both probed 2026-08-30).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/authentication/pennsylvania-state-university-authentication.yml
summary_line: apiKey/none/saml · 5 schemes
tags:
- Education
- Higher Education
- University
- Public Research University
- Land Grant
- Big Ten
- Research
- Research Data
- Research Repository
- Open Access
- Identity Federation
- Library
- Facilities
- United States
---
