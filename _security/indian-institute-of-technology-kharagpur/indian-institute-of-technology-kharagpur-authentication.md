---
api_key_in: []
api_specs:
- filename: indian-institute-of-technology-kharagpur-idr-opensearch-openapi.yml
  format: yaml
  label: IIT Kharagpur Institutional Digital Repository OpenSearch Interface
  slug: idr-opensearch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indian-institute-of-technology-kharagpur/refs/heads/main/openapi/indian-institute-of-technology-kharagpur-idr-opensearch-openapi.yml
- filename: indian-institute-of-technology-kharagpur-erp-cep-openapi.yml
  format: yaml
  label: IIT Kharagpur ERP Continuing Education Programme Brochure Endpoint
  slug: erp-cep-brochures
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indian-institute-of-technology-kharagpur/refs/heads/main/openapi/indian-institute-of-technology-kharagpur-erp-cep-openapi.yml
auth_types:
- none
- session
description: Authentication posture across IIT Kharagpur's surfaces. There is no API key issuance, no OAuth authorization server, no OpenID Connect discovery document and no published SAML metadata anywhere on the institute's public estate. The two callable surfaces recorded in this profile are entirely unauthenticated; everything else is behind an institute-built session SSO that is not federated and not documented.
kind: authentication
layout: security
method: probed
name: Indian Institute Of Technology Kharagpur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indian Institute of Technology Kharagpur secures its APIs with none and session across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Indian Institute of Technology Kharagpur
provider_slug: indian-institute-of-technology-kharagpur
scheme_count: 4
schemes:
- baseURL: http://www.idr.iitkgp.ac.in/xmlui/open-search/discover
  description: 'No authentication of any kind. Verified 2026-09-01 with a bare GET carrying no cookie, no Authorization header and no Referer — HTTP 200 with a full result feed. DSpace''s /login path exists for depositors but is irrelevant to reading. The transport is plain HTTP: the host has no TLS listener, so any credential sent to it would travel in the clear. Nothing about the read surface requires one.'
  name: idr-opensearch-anonymous
  surface: IIT Kharagpur Institutional Digital Repository OpenSearch interface
  type: none
  x-operator: institution
- baseURL: https://erp.iitkgp.ac.in/InfoCellDetails/resources/external/cepdata
  description: No authentication. The ERP sets a JSESSIONID cookie on the response but does not require one on the request; a first-contact GET with no cookie returns the PDF. This is the intent of the `external` path segment — the namespace exists so that the public institute website can link course brochures out of a system that is otherwise gated.
  name: erp-external-anonymous
  surface: IIT Kharagpur ERP Continuing Education Programme brochure endpoint
  type: none
  x-operator: institution
- description: 'Institute-built form/session SSO in front of the whole ERP. Requesting /InfoCellDetails/resources/application.wadl 302s to /SSOAdministration/login.htm?sessionToken=...&requestedUrl=..., i.e. the JAX-RS application does publish a WADL but it is only reachable to an authenticated session, so no machine contract can be read from outside. /SSOAdministration/auth.htm returns 405 to a GET (it expects POST). There is no OIDC discovery document, no token endpoint and no client-registration path: this is a private session cookie system, not an authorization server, and nothing on it is available to a third-party developer.'
  loginURL: https://erp.iitkgp.ac.in/SSOAdministration/login.htm
  name: erp-sso-session
  surface: IIT Kharagpur ERP (everything outside /resources/external)
  type: session
  x-operator: institution
- description: Separate session login guarding the HPC facility's allocation/accounting application. /robots.txt on the same host explicitly disallows /app/, /service/, /data/ and /HPC-Admin-User-Manual. No API, no token endpoint and no documentation are exposed.
  loginURL: https://hpc.iitkgp.ac.in/app
  name: hpc-app-session
  surface: HPC ERP System (PARAM Shakti allocation and job accounting)
  type: session
  x-operator: institution
slug: indian-institute-of-technology-kharagpur-authentication
source_filename: indian-institute-of-technology-kharagpur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes 2026-09-01 of http://www.idr.iitkgp.ac.in/xmlui/open-search/discover (200 with no\n  credentials), https://erp.iitkgp.ac.in/InfoCellDetails/resources/external/cepdata (200 with no\n  credentials), https://erp.iitkgp.ac.in/InfoCellDetails/resources/application.wadl (302 to\n  /SSOAdministration/login.htm), https://erp.iitkgp.ac.in/InfoCellDetails/ (403),\n  https://hpc.iitkgp.ac.in/app (login form), and the eduGAIN metadata database\n  (https://technical.edugain.org/api.php?action=list_entities).\nprovider: Indian Institute of Technology Kharagpur\nproviderId: indian-institute-of-technology-kharagpur\ndescription: >-\n  Authentication posture across IIT Kharagpur's surfaces. There is no API key issuance, no OAuth\n  authorization server, no OpenID Connect discovery document and no published SAML metadata\n  anywhere on the institute's public estate. The two callable surfaces recorded in this profile\n  are entirely\
  \ unauthenticated; everything else is behind an institute-built session SSO that is\n  not federated and not documented.\nsummary:\n  types: [none, session]\n  institution_operated: [none, session]\n  tenant_operated: []\n  key_issuance: none found\n  federated_identity: none found\nschemes:\n  - name: idr-opensearch-anonymous\n    type: none\n    x-operator: institution\n    surface: IIT Kharagpur Institutional Digital Repository OpenSearch interface\n    baseURL: http://www.idr.iitkgp.ac.in/xmlui/open-search/discover\n    description: >-\n      No authentication of any kind. Verified 2026-09-01 with a bare GET carrying no cookie, no\n      Authorization header and no Referer — HTTP 200 with a full result feed. DSpace's /login\n      path exists for depositors but is irrelevant to reading. The transport is plain HTTP: the\n      host has no TLS listener, so any credential sent to it would travel in the clear. Nothing\n      about the read surface requires one.\n  - name: erp-external-anonymous\n\
  \    type: none\n    x-operator: institution\n    surface: IIT Kharagpur ERP Continuing Education Programme brochure endpoint\n    baseURL: https://erp.iitkgp.ac.in/InfoCellDetails/resources/external/cepdata\n    description: >-\n      No authentication. The ERP sets a JSESSIONID cookie on the response but does not require\n      one on the request; a first-contact GET with no cookie returns the PDF. This is the intent\n      of the `external` path segment — the namespace exists so that the public institute website\n      can link course brochures out of a system that is otherwise gated.\n  - name: erp-sso-session\n    type: session\n    x-operator: institution\n    surface: IIT Kharagpur ERP (everything outside /resources/external)\n    loginURL: https://erp.iitkgp.ac.in/SSOAdministration/login.htm\n    description: >-\n      Institute-built form/session SSO in front of the whole ERP. Requesting\n      /InfoCellDetails/resources/application.wadl 302s to\n      /SSOAdministration/login.htm?sessionToken=...&requestedUrl=...,\
  \ i.e. the JAX-RS application\n      does publish a WADL but it is only reachable to an authenticated session, so no machine\n      contract can be read from outside. /SSOAdministration/auth.htm returns 405 to a GET\n      (it expects POST). There is no OIDC discovery document, no token endpoint and no\n      client-registration path: this is a private session cookie system, not an authorization\n      server, and nothing on it is available to a third-party developer.\n  - name: hpc-app-session\n    type: session\n    x-operator: institution\n    surface: HPC ERP System (PARAM Shakti allocation and job accounting)\n    loginURL: https://hpc.iitkgp.ac.in/app\n    description: >-\n      Separate session login guarding the HPC facility's allocation/accounting application.\n      /robots.txt on the same host explicitly disallows /app/, /service/, /data/ and\n      /HPC-Admin-User-Manual. No API, no token endpoint and no documentation are exposed.\nnotes:\n  - >-\n    No Shibboleth or SAML\
  \ identity provider for iitkgp.ac.in exists in the eduGAIN metadata\n    database. India's national federation INFED (registration authority http://inflibnet.ac.in,\n    an eduGAIN member since 2017) publishes 379 entities and none of them carries an iitkgp.ac.in\n    entityID or a Kharagpur display name — checked against the full 10,616-entity eduGAIN export\n    on 2026-09-01. Peer IITs are present (e.g. https://identity.iith.ac.in/idp/shibboleth for\n    IIT Hyderabad), so the absence is a real gap rather than a national one.\n  - >-\n    No .well-known directory of any kind was found. https://www.iitkgp.ac.in/.well-known/security.txt\n    returns HTTP 200 but serves the site's Angular shell (47,510 bytes, byte-identical to the\n    homepage response) — a soft 404, not a security.txt. It is recorded as absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indian-institute-of-technology-kharagpur/refs/heads/main/authentication/indian-institute-of-technology-kharagpur-authentication.yml
summary_line: none/session · 4 schemes
tags:
- Education
- Higher Education
- University
- Institute of Technology
- India
- Research
- Research Repository
- Institutional Repository
- DSpace
- OpenSearch
- Course Catalog
- Research Computing
- Library
---
