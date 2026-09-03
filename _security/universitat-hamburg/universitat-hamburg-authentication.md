---
api_key_in: []
api_specs:
- filename: universitat-hamburg-zfdm-repository-openapi.yml
  format: yaml
  label: ZFDM Research Data Repository API
  slug: zfdm-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universitat-hamburg/refs/heads/main/openapi/universitat-hamburg-zfdm-repository-openapi.yml
auth_types: []
description: Universität Hamburg's public read surfaces are open and unauthenticated. Write access to the research-data repository, and access to every campus system, runs through the institution's own Shibboleth/SAML 2.0 Identity Provider — which is itself the institution's strongest machine-readable surface.
kind: authentication
layout: security
method: probed
name: Universitat Hamburg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Universität Hamburg declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Universität Hamburg
provider_slug: universitat-hamburg
scheme_count: 3
schemes:
- applies_to:
  - https://www.fdr.uni-hamburg.de/api (read paths)
  - https://www.fdr.uni-hamburg.de/oai2d
  - https://ediss.sub.uni-hamburg.de/oai/request
  - https://hup.sub.uni-hamburg.de/index.php/index/oai
  - https://journals.sub.uni-hamburg.de/index.php/index/oai
  - https://digitalisate.sub.uni-hamburg.de/oai
  detail: 'No credential of any kind is required. Verified 2026-09-01: all six return 200 with no Authorization header sent. The ZFDM API additionally sets `Access-Control-Allow-Origin: *`, so browser clients can call it directly.'
  name: none
- applies_to:
  - https://www.fdr.uni-hamburg.de/api/deposit/depositions
  detail: Deposit (write) paths are credentialed. Verified 2026-09-01 returning HTTP 401 with a JSON body stating that the server could not verify authorization. Token issuance is account-based and is not self-service; no public registration flow was found.
  name: bearer-token
- applies_to:
  - STiNE campus management (https://www.stine.uni-hamburg.de/)
  - RRZ GitLab (https://gitlab.rrz.uni-hamburg.de/)
  - Licensed library and e-resource services
  detail: Federated single sign-on via the institution's own Shibboleth IdP, entityID https://login.uni-hamburg.de/idp/shibboleth, registered in DFN-AAI (registrationAuthority https://www.aai.dfn.de) and thereby in eduGAIN. Metadata is served at the entityID URL and via the DFN-AAI MDQ service. The IdP asserts support for the REFEDS Research & Scholarship entity category and the GÉANT Data Protection Code of Conduct v1.
  federation: DFN-AAI (eduGAIN)
  metadata_url: https://login.uni-hamburg.de/idp/shibboleth
  name: saml2-shibboleth
slug: universitat-hamburg-authentication
source_filename: universitat-hamburg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Universität Hamburg\nproviderId: universitat-hamburg\ngenerated: '2026-09-01'\nmethod: probed\nsource:\n  - https://www.fdr.uni-hamburg.de/api/records/?size=1\n  - https://www.fdr.uni-hamburg.de/api/deposit/depositions\n  - https://ediss.sub.uni-hamburg.de/oai/request?verb=Identify\n  - https://login.uni-hamburg.de/idp/shibboleth\n  - https://www.rrz.uni-hamburg.de/services/weitere/authentifizierung/shibboleth/configure.html\ndescription: >-\n  Universität Hamburg's public read surfaces are open and unauthenticated. Write\n  access to the research-data repository, and access to every campus system,\n  runs through the institution's own Shibboleth/SAML 2.0 Identity Provider —\n  which is itself the institution's strongest machine-readable surface.\nschemes:\n  - name: none\n    applies_to:\n      - https://www.fdr.uni-hamburg.de/api (read paths)\n      - https://www.fdr.uni-hamburg.de/oai2d\n \
  \     - https://ediss.sub.uni-hamburg.de/oai/request\n      - https://hup.sub.uni-hamburg.de/index.php/index/oai\n      - https://journals.sub.uni-hamburg.de/index.php/index/oai\n      - https://digitalisate.sub.uni-hamburg.de/oai\n    detail: >-\n      No credential of any kind is required. Verified 2026-09-01: all six return\n      200 with no Authorization header sent. The ZFDM API additionally sets\n      `Access-Control-Allow-Origin: *`, so browser clients can call it directly.\n  - name: bearer-token\n    applies_to:\n      - https://www.fdr.uni-hamburg.de/api/deposit/depositions\n    detail: >-\n      Deposit (write) paths are credentialed. Verified 2026-09-01 returning\n      HTTP 401 with a JSON body stating that the server could not verify\n      authorization. Token issuance is account-based and is not self-service;\n      no public registration flow was found.\n  - name: saml2-shibboleth\n    applies_to:\n      - STiNE campus management (https://www.stine.uni-hamburg.de/)\n\
  \      - RRZ GitLab (https://gitlab.rrz.uni-hamburg.de/)\n      - Licensed library and e-resource services\n    detail: >-\n      Federated single sign-on via the institution's own Shibboleth IdP,\n      entityID https://login.uni-hamburg.de/idp/shibboleth, registered in DFN-AAI\n      (registrationAuthority https://www.aai.dfn.de) and thereby in eduGAIN.\n      Metadata is served at the entityID URL and via the DFN-AAI MDQ service.\n      The IdP asserts support for the REFEDS Research & Scholarship entity\n      category and the GÉANT Data Protection Code of Conduct v1.\n    metadata_url: https://login.uni-hamburg.de/idp/shibboleth\n    federation: DFN-AAI (eduGAIN)\nnot_offered:\n  - oauth2_authorization_code\n  - oauth2_client_credentials\n  - dynamic_client_registration\n  - api_key_self_service\nnotes: >-\n  No OAuth 2.0 authorization server, no RFC 9728 protected-resource metadata and\n  no /.well-known catalog were found on any uni-hamburg.de host; /llms.txt and\n  /.well-known/security.txt\
  \ on www.uni-hamburg.de both return 404.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universitat-hamburg/refs/heads/main/authentication/universitat-hamburg-authentication.yml
summary_line: 3 schemes
tags:
- Education
- Higher Education
- University
- Germany
- Research Data
- Research Repository
- Library
- Open Access
- Metadata
- OAI-PMH
- Identity Federation
- DataCite
---
