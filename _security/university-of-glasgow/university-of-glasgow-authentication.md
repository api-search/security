---
api_key_in: []
api_specs:
- filename: university-of-glasgow-enlighten-rest-openapi.yml
  format: yaml
  label: Enlighten EPrints REST API
  slug: enlighten-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-glasgow/refs/heads/main/openapi/university-of-glasgow-enlighten-rest-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: University Of Glasgow Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Glasgow declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Glasgow
provider_slug: university-of-glasgow
scheme_count: 0
schemes: []
slug: university-of-glasgow-authentication
source_filename: university-of-glasgow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: University of Glasgow — authentication posture\naid: university-of-glasgow\ngenerated: '2026-08-30'\nmethod: derived\nx-evidence-method: probed\nsource: live probes of University of Glasgow operated hosts, 2026-08-30\nsummary: >-\n  Every machine-readable surface the University of Glasgow operates and exposes to the public is\n  open and unauthenticated: three OAI-PMH endpoints and the read side of the Enlighten EPrints REST\n  interface all answer anonymously. Everything the institution gates, it gates through one\n  mechanism — the GUID single sign-on estate behind its Shibboleth SAML 2.0 identity provider. That\n  identity provider is by some distance the institution's largest and best-maintained machine-readable\n  artifact, and it is a login federation rather than a programmable API, which is the honest shape of\n  most of this cohort.\napis:\n- aid: university-of-glasgow:enlighten-oai\n  x-operator: institution\n  scheme: none\n  detail: >-\n    OAI-PMH is an open\
  \ harvesting protocol. verb=Identify, verb=ListMetadataFormats and\n    verb=ListRecords all returned 200 with real data and no credential on 2026-08-30.\n  verified: '2026-08-30'\n- aid: university-of-glasgow:researchdata-oai\n  x-operator: institution\n  scheme: none\n  detail: >-\n    Anonymous verb=ListRecords returned a 266 KB page of live dataset records carrying DOIs under\n    prefix 10.5525 on 2026-08-30.\n  verified: '2026-08-30'\n- aid: university-of-glasgow:theses-oai\n  x-operator: institution\n  scheme: none\n  detail: Anonymous verb=Identify returned repositoryName \"Enlighten Theses\" on 2026-08-30.\n  verified: '2026-08-30'\n- aid: university-of-glasgow:enlighten-rest\n  x-operator: institution\n  scheme: http-basic\n  public_read: true\n  detail: >-\n    Read access to the dataset indexes, eprint records and subject taxonomy is anonymous — /rest/,\n    /rest/eprint/, /rest/eprint/1.xml, /rest/eprint/1/title.txt and /rest/subject/ all returned 200\n    without credentials\
  \ on 2026-08-30. The user dataset is the exception: /rest/user/ lists\n    identifiers only and /rest/user/1.xml returned 401, so no personal data is reachable anonymously.\n    EPrints HTTP Basic credentials are required for user records and for any write. There is no\n    OAuth, no API key, no token endpoint and no scope model.\n  verified: '2026-08-30'\n- aid: university-of-glasgow:moodle-lti\n  x-operator: institution\n  x-vendor: moodle\n  scheme: oauth2-jwt\n  detail: >-\n    The virtual learning environment's LTI 1.3 platform surface is machine-readable but not open:\n    /mod/lti/certs.php serves the public JWKS anonymously (200), while /mod/lti/token.php returns\n    400 to an unsigned request and the Moodle Web Services REST endpoint at\n    /webservice/rest/server.php returns a Moodle invalidtoken exception. Access is by\n    registered-tool client credentials issued by the institution, not by public self-service. The\n    scheme is Moodle's, not Glasgow's engineering.\n  verified:\
  \ '2026-08-30'\n- aid: university-of-glasgow:sierra-library-api\n  x-operator: institution\n  x-vendor: innovative-interfaces\n  scheme: oauth2-client-credentials\n  detail: >-\n    The library management system at eleanor.lib.gla.ac.uk exposes the Innovative Interfaces Sierra\n    API. /iii/sierra-api/v6/info/token returned 401 on 2026-08-30 — live and credentialed, not\n    absent. Keys are issued by the library to named partners; there is no public registration path.\n  verified: '2026-08-30'\n- aid: university-of-glasgow:worldcat-discovery\n  x-operator: tenant\n  x-vendor: oclc\n  scheme: vendor\n  detail: >-\n    gla.on.worldcat.org is Glasgow's OCLC WorldCat Discovery tenancy. Any programmatic access runs\n    on OCLC's own WorldCat Search API keys and OAuth, documented and operated by OCLC. Not scored\n    here.\n  verified: '2026-08-30'\n- aid: university-of-glasgow:libguides\n  x-operator: tenant\n  x-vendor: springshare\n  scheme: vendor\n  detail: >-\n    gla.libguides.com\
  \ is Glasgow's Springshare LibGuides tenancy. The LibGuides API is Springshare's\n    product, keyed per site by Springshare. Not scored here.\n  verified: '2026-08-30'\nidentity_federation:\n  x-operator: institution\n  protocol: SAML 2.0 / Shibboleth\n  entity_id: https://idp.gla.ac.uk/shibboleth\n  scope: gla.ac.uk\n  metadata:\n    self_published: https://idp.gla.ac.uk/idp/shibboleth\n    federation_mdq: http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fidp.gla.ac.uk%2Fshibboleth\n  federations:\n  - UK Access Management Federation\n  - eduGAIN\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:mace:shibboleth:1.0:profiles:AuthnRequest\n  entities_registered: 2\n  service_providers_registered: 0\n  detail: >-\n    Glasgow registers a production IdP and a test IdP (https://idptest.gla.ac.uk/idp/shibboleth) in\n    the UK federation aggregate\
  \ and no Service Provider entities. Both metadata copies — the IdP's\n    own and the federation's signed MDQ copy — were fetched and read on 2026-08-30.\n  verified: '2026-08-30'\nnotes:\n- >-\n  No developer key, no OAuth client registration, no API key issuance page and no self-service\n  onboarding of any kind exists on gla.ac.uk. Everything credentialed here is credentialed through\n  institutional identity or a library/VLE administrator.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-glasgow/refs/heads/main/authentication/university-of-glasgow-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Scotland
- Russell Group
- Research Data
- Repository
- OAI-PMH
- Open Access
- Identity Federation
- Digital Library
---
