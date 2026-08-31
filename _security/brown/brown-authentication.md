---
api_key_in: []
api_specs:
- filename: brown-bdr-api-openapi.yml
  format: yaml
  label: Brown Digital Repository (BDR) API
  slug: bdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brown/refs/heads/main/openapi/brown-bdr-api-openapi.yml
- filename: brown-bdr-iiif-openapi.yml
  format: yaml
  label: Brown Digital Repository IIIF Image and Presentation API
  slug: bdr-iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brown/refs/heads/main/openapi/brown-bdr-iiif-openapi.yml
auth_types: []
description: 'Brown''s programmable surface has two authentication stories and they do not meet. The public BDR API has no authentication at all — no key, no OAuth, no registration, nothing to obtain. The institution''s real identity infrastructure is a SAML 2.0 Shibboleth identity provider registered in InCommon, which is a browser SSO protocol and is not usable as API credentials. There is no bridge: no OAuth authorization server, no token endpoint, no OIDC discovery document, no dynamic client registration, no protected-resource metadata. An agent or a script cannot authenticate to anything at Brown; it can only read what is already public.'
kind: authentication
layout: security
method: derived
name: Brown Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brown University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Brown University
provider_slug: brown
scheme_count: 0
schemes: []
slug: brown-authentication
source_filename: brown-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: Brown University\nproviderId: brown\ngenerated: '2026-08-30'\nmethod: derived\nprobed: '2026-08-30'\nmethod_note: >-\n  Authored by API Evangelist from live probes on 2026-08-30, not published by Brown. `derived` is the\n  authorship class the catalog's provenance manifest reads; the probe evidence itself is in `source`\n  and in the per-finding `evidence` blocks below.\nsource:\n- https://repository.library.brown.edu/api/search/?q=*&rows=1\n- https://repository.library.brown.edu/api/login/\n- https://sso.brown.edu/idp/shibboleth\n- https://mdq.incommon.org/entities/https%3A%2F%2Fsso.brown.edu%2Fidp%2Fshibboleth\n- https://ithelp.brown.edu/kb/shibboleth-single-sign-on\ndescription: >-\n  Brown's programmable surface has two authentication stories and they do not meet. The public BDR\n  API has no authentication at all — no key, no OAuth, no registration, nothing to obtain. The\n  institution's\
  \ real identity infrastructure is a SAML 2.0 Shibboleth identity provider registered in\n  InCommon, which is a browser SSO protocol and is not usable as API credentials. There is no bridge:\n  no OAuth authorization server, no token endpoint, no OIDC discovery document, no dynamic client\n  registration, no protected-resource metadata. An agent or a script cannot authenticate to anything\n  at Brown; it can only read what is already public.\nsurfaces:\n- name: Brown Digital Repository (BDR) API\n  x-operator: institution\n  scheme: none\n  registration: not applicable\n  evidence:\n    url: https://repository.library.brown.edu/api/search/?q=*&rows=1\n    status: 200\n    note: Returned 200 and a full result set with no credential of any kind.\n  boundary: >-\n    The access boundary is visibility, not authentication. Every indexed object carries\n    `_display_public_bsi`, `_display_brown_bsi` and `_display_private_bsi`; the anonymous API sees\n    the public set. Every search response\
  \ includes a `links.login` URL pointing at\n    `https://repository.library.brown.edu/api/login/?next=<the same query>`, which is the API\n    telling a caller that a larger, Brown-authenticated view of that exact query exists. That login\n    is a browser Shibboleth redirect, not a token grant.\n- name: Brown Shibboleth Identity Provider\n  x-operator: institution\n  scheme: SAML 2.0 web browser SSO\n  entityID: https://sso.brown.edu/idp/shibboleth\n  evidence:\n    url: https://sso.brown.edu/idp/shibboleth\n    status: 200\n    content_type: application/xml;charset=UTF-8\n    bytes: 5652\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST -> https://sso.brown.edu/idp/profile/SAML2/POST/SSO\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect -> https://sso.brown.edu/idp/profile/SAML2/Redirect/SSO\n  - urn:mace:shibboleth:1.0:profiles:AuthnRequest -> https://sso.brown.edu/idp/profile/Shibboleth/SSO\n  scope: brown.edu\n  note: >-\n    Machine-readable and self-published,\
  \ which is rare — most institutions leave their IdP metadata\n    to the federation aggregate. It is nonetheless a human-browser protocol. It grants no API access.\nabsent:\n  oauth2: true\n  openid_connect_discovery: true\n  api_keys: true\n  dynamic_client_registration: true\n  protected_resource_metadata: true\n  delegated_identity: true\n  service_accounts: true\n  note: >-\n    Probed and not found. Recorded as absent rather than omitted, because absence here is the\n    finding: Brown publishes a strong institutional identity contract and no way for software to use it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brown/refs/heads/main/authentication/brown-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- United States
- Ivy League
- Research
- Research Repository
- Digital Repository
- Library
- IIIF
- Identity Federation
- Course Catalog
- Research Computing
---
