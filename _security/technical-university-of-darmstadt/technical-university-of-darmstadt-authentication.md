---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Technical University Of Darmstadt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Technical University of Darmstadt declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Technical University of Darmstadt
provider_slug: technical-university-of-darmstadt
scheme_count: 0
schemes: []
slug: technical-university-of-darmstadt-authentication
source_filename: technical-university-of-darmstadt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\n# How authentication works across TU Darmstadt's programmable surfaces.\n# Derived from the institution's own live SAML metadata and from live probes of each\n# surface; nothing here is inferred from documentation alone.\nslug: technical-university-of-darmstadt\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://idp.hrz.tu-darmstadt.de/idp/shibboleth (fetched 2026-09-01, HTTP 200,\n  15,371 bytes of SAML 2.0 metadata) plus unauthenticated probes of each listed surface.\nprimary:\n  type: saml2-shibboleth\n  operator: institution\n  entity_id: https://idp.hrz.tu-darmstadt.de/idp/shibboleth\n  metadata_url: https://idp.hrz.tu-darmstadt.de/idp/shibboleth\n  scope: tu-darmstadt.de\n  federation: DFN-AAI (Deutsches Forschungsnetz), reachable via eduGAIN\n  federation_mdq: https://mdq.aai.dfn.de/entities/\n  operated_by: Hochschulrechenzentrum (HRZ), TU Darmstadt\n  contacts:\n    technical: idmadmin@hrz.tu-darmstadt.de\n    support: service@hrz.tu-darmstadt.de\n\
  \  endpoints:\n    - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n      location: https://login.tu-darmstadt.de/idp/profile/Shibboleth/SSO\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      location: https://login.tu-darmstadt.de/idp/profile/SAML2/POST/SSO\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n      location: https://login.tu-darmstadt.de/idp/profile/SAML2/POST-SimpleSign/SSO\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      location: https://login.tu-darmstadt.de/idp/profile/SAML2/Redirect/SSO\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n      location: https://login.tu-darmstadt.de/idp/profile/SAML2/SOAP/ECP\n      note: ECP profile — the one binding here usable by a non-browser client.\n  notes: >-\n    This is browser-mediated web SSO for humans. It is not an API authorization\n    server: there is no OAuth 2.0 or OpenID Connect token endpoint published on the\n    institution's\
  \ public surface, and no RFC 9728 protected-resource metadata was\n    found. An agent cannot obtain a bearer token here.\nsurfaces:\n  - surface: TUdatalib DSpace REST API\n    base_url: https://tudatalib.ulb.tu-darmstadt.de/server/api\n    anonymous_read: true\n    scheme: >-\n      Anonymous GET works for the API root and public discovery. Write and restricted\n      reads use DSpace's own /server/api/authn endpoints, which chain to the\n      Shibboleth IdP above.\n    method: probed\n  - surface: TUdatalib OAI-PMH\n    base_url: https://tudatalib.ulb.tu-darmstadt.de/server/oai/request\n    anonymous_read: true\n    scheme: None. OAI-PMH is unauthenticated by protocol.\n    method: probed\n  - surface: DBRepo API v1\n    base_url: https://dbrepo.ulb.tu-darmstadt.de/api/v1\n    anonymous_read: true\n    scheme: >-\n      Public database listings and the license vocabulary return 200 anonymously.\n      DBRepo's write and private paths use a Keycloak-issued bearer token; no\n      registration\
  \ path was found on the public surface.\n    method: probed\n  - surface: TUjournals (Janeway) REST API\n    base_url: https://tujournals.ulb.tu-darmstadt.de/api\n    anonymous_read: true\n    scheme: >-\n      Fully anonymous read across /api/journals/, /api/articles/ and /api/issues/.\n      Note the operator is a vendor (Janeway shared hosting), not the institution.\n    method: probed\nnot_found:\n  - oauth2\n  - openid-connect\n  - api-keys\n  - rfc9728-protected-resource-metadata\n  - developer-registration-portal\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/technical-university-of-darmstadt/refs/heads/main/authentication/technical-university-of-darmstadt-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Technical University
- Germany
- Research Data
- Open Access
- Scholarly Publishing
- Library
- OAI-PMH
- DSpace
- Identity Federation
- Shibboleth
- Research Computing
---
