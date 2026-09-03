---
api_key_in: []
auth_types:
- saml2
- cas
- oauth2
- none
description: ''
kind: authentication
layout: security
method: probed
name: Arizona State University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arizona State University secures its APIs with saml2, cas, oauth2, and none across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Arizona State University
provider_slug: arizona-state-university
scheme_count: 4
schemes:
- description: ASU's Shibboleth Identity Provider, entityID urn:mace:incommon:asu.edu, asserting the scope asu.edu. Registered in the InCommon Federation and published as signed, machine-readable SAML metadata through the InCommon MDQ service; ASU also serves its own entity descriptor from its own host. This is institutional single sign-on infrastructure, not a developer API — no application can obtain an assertion without being registered as a service provider in the federation.
  display_name: Arizona State University
  endpoints:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://shibboleth2.asu.edu/idp/profile/SAML2/Redirect/SSO
    role: SingleSignOnService
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://shibboleth2.asu.edu/idp/profile/SAML2/POST/SSO
    role: SingleSignOnService
  entity_id: urn:mace:incommon:asu.edu
  information_url: https://www.asu.edu/about
  local_copy: authentication/arizona-state-university-saml-idp-metadata.xml
  metadata:
  - detail: Signed EntityDescriptor, 6702 bytes, retrieved 2026-09-01.
    location: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aasu.edu
    status: 200
  - detail: ASU's own metadata endpoint on ASU's own host, 1559 bytes, application/xml. Institution-served federation metadata — the strongest evidence that the IdP is ASU-operated rather than bought.
    location: https://shibboleth2.asu.edu/idp/shibboleth
    status: 200
  name: shibboleth-saml2
  organization_name: Arizona State University
  privacy_statement_url: https://www.asu.edu/privacy/
  protocols:
  - urn:oasis:names:tc:SAML:2.0:protocol
  scope: asu.edu
  type: saml2
  x-operator: institution
- base_url: https://weblogin.asu.edu/cas
  description: ASU WebAuth, a Central Authentication Service (CAS) deployment used to authenticate ASURITE accounts across university web applications. Integration is restricted to ASU-approved service providers; there is no self-service registration.
  name: asu-webauth-cas
  probe:
    detail: Returns a Spring Boot YAML error body (status 401, "Unauthorized", path /cas) to a bare unauthenticated GET. Live and protocol-correct, not an outage and not a soft 404.
    location: https://weblogin.asu.edu/cas
    probed: '2026-09-01'
    status: 401
  type: cas
  x-operator: institution
- base_url: https://eadvs-cscc-catalog-api.apps.asu.edu/catalog-microservices/api/v1
  description: The ASU course catalog single-page application authenticates to its own backend (eadvs-cscc-catalog-api.apps.asu.edu) with an OAuth 2.0 bearer token obtained against an ASU client_id. No token endpoint, scope list or client registration is published for outside developers, and every catalog-microservices path returns 401 without one.
  known_scopes:
  - https://api.myasuplat-dpl.asu.edu/scopes/acad-plan/read
  - https://api.myasuplat-dpl.asu.edu/scopes/person/read
  - https://api.myasuplat-dpl.asu.edu/scopes/principal/read
  name: catalog-microservices-oauth2
  probe:
    detail: text/plain "Unauthorized", 12 bytes. A negative probe against /catalog-microservices/api/v1/NOT-REAL returns 404 "Not found", so the 401 is a real authorization boundary and not a catch-all.
    location: https://eadvs-cscc-catalog-api.apps.asu.edu/catalog-microservices/api/v1/search/terms
    probed: '2026-09-01'
    status: 401
  scopes_source: Scope URIs read out of the public catalog SPA bundle https://catalog.apps.asu.edu/assets/index-BkWV8O6a.js (200, 2342417 bytes, retrieved 2026-09-01). Recorded as observed strings, not as a published scope catalogue.
  type: oauth2
  x-operator: institution
- description: 'The four surfaces an outside agent can call with no credentials at all: the ASU Dataverse read API, and the OAI-PMH 2.0 endpoints of ASU Dataverse, KEEP and PRISM.'
  endpoints:
  - https://dataverse.asu.edu/api
  - https://dataverse.asu.edu/oai
  - https://keep.lib.asu.edu/oai/request
  - https://prism.lib.asu.edu/oai/request
  name: anonymous
  type: none
  x-operator: institution
slug: arizona-state-university-authentication
source_filename: arizona-state-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of Arizona State University's own authentication surfaces, plus the\n  institution's signed SAML entity descriptor retrieved from the InCommon MDQ service and from\n  ASU's own metadata endpoint at shibboleth2.asu.edu.\nx-operator: institution\n\nsummary:\n  note: >-\n    ASU operates no public OAuth authorization server and issues no self-service API credentials.\n    Its institution-operated authentication is federated SAML (Shibboleth) plus CAS for people, and\n    an internal OAuth 2.0 bearer scheme in front of the course-catalog microservices and the myASU\n    data platform that only ASU-registered clients can obtain a token from. The machine surfaces an\n    outside agent can actually call anonymously are the three OAI-PMH endpoints and the Dataverse\n    read API; everything else is closed.\n  types:\n  - saml2\n  - cas\n  - oauth2\n  - none\n  public_oauth: false\n  self_serve_api_keys:\
  \ false\n\nschemes:\n- name: shibboleth-saml2\n  type: saml2\n  x-operator: institution\n  description: >-\n    ASU's Shibboleth Identity Provider, entityID urn:mace:incommon:asu.edu, asserting the scope\n    asu.edu. Registered in the InCommon Federation and published as signed, machine-readable SAML\n    metadata through the InCommon MDQ service; ASU also serves its own entity descriptor from its\n    own host. This is institutional single sign-on infrastructure, not a developer API — no\n    application can obtain an assertion without being registered as a service provider in the\n    federation.\n  entity_id: urn:mace:incommon:asu.edu\n  scope: asu.edu\n  organization_name: Arizona State University\n  display_name: Arizona State University\n  protocols:\n  - urn:oasis:names:tc:SAML:2.0:protocol\n  endpoints:\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    location: https://shibboleth2.asu.edu/idp/profile/SAML2/Redirect/SSO\n    role: SingleSignOnService\n  - binding:\
  \ urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    location: https://shibboleth2.asu.edu/idp/profile/SAML2/POST/SSO\n    role: SingleSignOnService\n  metadata:\n  - location: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aasu.edu\n    status: 200\n    detail: Signed EntityDescriptor, 6702 bytes, retrieved 2026-09-01.\n  - location: https://shibboleth2.asu.edu/idp/shibboleth\n    status: 200\n    detail: >-\n      ASU's own metadata endpoint on ASU's own host, 1559 bytes, application/xml. Institution-served\n      federation metadata — the strongest evidence that the IdP is ASU-operated rather than bought.\n  local_copy: authentication/arizona-state-university-saml-idp-metadata.xml\n  information_url: https://www.asu.edu/about\n  privacy_statement_url: https://www.asu.edu/privacy/\n\n- name: asu-webauth-cas\n  type: cas\n  x-operator: institution\n  description: >-\n    ASU WebAuth, a Central Authentication Service (CAS) deployment used to authenticate ASURITE\n    accounts\
  \ across university web applications. Integration is restricted to ASU-approved service\n    providers; there is no self-service registration.\n  base_url: https://weblogin.asu.edu/cas\n  probe:\n    location: https://weblogin.asu.edu/cas\n    status: 401\n    detail: >-\n      Returns a Spring Boot YAML error body (status 401, \"Unauthorized\", path /cas) to a bare\n      unauthenticated GET. Live and protocol-correct, not an outage and not a soft 404.\n    probed: '2026-09-01'\n\n- name: catalog-microservices-oauth2\n  type: oauth2\n  x-operator: institution\n  description: >-\n    The ASU course catalog single-page application authenticates to its own backend\n    (eadvs-cscc-catalog-api.apps.asu.edu) with an OAuth 2.0 bearer token obtained against an ASU\n    client_id. No token endpoint, scope list or client registration is published for outside\n    developers, and every catalog-microservices path returns 401 without one.\n  base_url: https://eadvs-cscc-catalog-api.apps.asu.edu/catalog-microservices/api/v1\n\
  \  probe:\n    location: https://eadvs-cscc-catalog-api.apps.asu.edu/catalog-microservices/api/v1/search/terms\n    status: 401\n    detail: >-\n      text/plain \"Unauthorized\", 12 bytes. A negative probe against\n      /catalog-microservices/api/v1/NOT-REAL returns 404 \"Not found\", so the 401 is a real\n      authorization boundary and not a catch-all.\n    probed: '2026-09-01'\n  known_scopes:\n  - https://api.myasuplat-dpl.asu.edu/scopes/acad-plan/read\n  - https://api.myasuplat-dpl.asu.edu/scopes/person/read\n  - https://api.myasuplat-dpl.asu.edu/scopes/principal/read\n  scopes_source: >-\n    Scope URIs read out of the public catalog SPA bundle\n    https://catalog.apps.asu.edu/assets/index-BkWV8O6a.js (200, 2342417 bytes, retrieved\n    2026-09-01). Recorded as observed strings, not as a published scope catalogue.\n\n- name: anonymous\n  type: none\n  x-operator: institution\n  description: >-\n    The four surfaces an outside agent can call with no credentials at all: the ASU\
  \ Dataverse read\n    API, and the OAI-PMH 2.0 endpoints of ASU Dataverse, KEEP and PRISM.\n  endpoints:\n  - https://dataverse.asu.edu/api\n  - https://dataverse.asu.edu/oai\n  - https://keep.lib.asu.edu/oai/request\n  - https://prism.lib.asu.edu/oai/request\n\nnot_found:\n  note: >-\n    Probed and absent on 2026-09-01, recorded so a later run does not re-hunt them.\n  hosts_that_do_not_resolve:\n  - api.asu.edu\n  - data.asu.edu\n  - open.asu.edu\n  - developer.asu.edu\n  - status.asu.edu\n  no_public_developer_portal: true\n  no_self_service_api_keys: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arizona-state-university/refs/heads/main/authentication/arizona-state-university-authentication.yml
summary_line: saml2/cas/oauth2/none · 4 schemes
tags:
- University
- Higher Education
- Education
- United States
- Arizona
- Public Research University
- Research Data
- Research Repository
- Identity Federation
- OAI-PMH
- Course Catalog
- Library
---
