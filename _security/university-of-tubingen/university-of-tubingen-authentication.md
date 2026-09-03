---
api_key_in: []
auth_types:
- none
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: University Of Tubingen Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Tübingen secures its APIs with none and saml2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Tübingen
provider_slug: university-of-tubingen
scheme_count: 2
schemes:
- description: 'Public read access with no credential of any kind. GET https://fdat.uni-tuebingen.de/api/records?size=1 returns 200 application/json (437 records); GET https://fdat.uni-tuebingen.de/api/records/zvknn-g0x34 returns 200 with ETag "6" and a Link rel="linkset" header; GET https://fdat.uni-tuebingen.de/api/communities?size=1 and /api/vocabularies/languages?size=1 both return 200. Both OAI-PMH providers answer verb=Identify with 200 text/xml unauthenticated. Server-side throttling is advertised rather than authentication — X-RateLimit-Limit: 500, X-RateLimit-Remaining, X-RateLimit-Reset and Retry-After: 60 are returned on FDAT API responses. Note that https://fdat.uni-tuebingen.de/robots.txt disallows /api and /search for crawlers with Crawl-delay: 10; the API is open to clients but the operator does not invite bulk crawling.'
  name: anonymous-read
  sources:
  - https://fdat.uni-tuebingen.de/api/records
  - https://fdat.uni-tuebingen.de/oai2d?verb=Identify
  - https://publikationen.uni-tuebingen.de/oai/request?verb=Identify
  type: none
- description: 'Institutional single sign-on through the university''s own Shibboleth Identity Provider, entityID https://idp.uni-tuebingen.de/shibboleth, scope uni-tuebingen.de, registered in DFN-AAI since 2009-05-26 and exported to eduGAIN. SSO endpoints: HTTP-POST https://idp.uni-tuebingen.de/idp/profile/SAML2/POST/SSO, HTTP-Redirect https://idp.uni-tuebingen.de/idp/profile/SAML2/Redirect/SSO, SOAP/ECP https://idp.uni-tuebingen.de/idp/profile/SAML2/SOAP/ECP. NameID formats: persistent and transient. A SAML 2.0 AttributeAuthorityDescriptor with a SOAP AttributeService is also published. The entity asserts REFEDS Research & Scholarship support and SIRTFI + SIRTFI2 assurance certification, and is a bwIDM member (the Baden-Württemberg federated identity programme). Relying parties obtain the signing key and endpoints from federation metadata, not from the university — this is a federated trust surface, not a self-service API credential.'
  name: shibboleth-saml2-sso
  sources:
  - https://mdq.aai.dfn.de/entities/https%3A%2F%2Fidp.uni-tuebingen.de%2Fshibboleth
  - https://uni-tuebingen.de/en/einrichtungen/zentrum-fuer-datenverarbeitung/dienstleistungen/digitale-identitaet/single-sign-on/
  type: saml2
slug: university-of-tubingen-authentication
source_filename: university-of-tubingen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes of University of Tübingen institution-operated hosts on 2026-09-01, plus the\n  DFN-AAI SAML MDQ service. Not derived from any OpenAPI — the institution publishes none.\nnote: >-\n  Two authentication postures, and they are opposites. Every machine-readable surface the university\n  actually operates for the public — the FDAT REST API, both OAI-PMH providers — is ANONYMOUS: no key,\n  no registration, no self-service credential issuance anywhere on the institution's public estate.\n  Everything else — campus management (alma), the VLE, storage, the licensed library estate — is\n  behind institutional SSO, which is SAML 2.0 via the university's own Shibboleth IdP registered in\n  DFN-AAI. There is no OAuth 2.0 authorization server, no OpenID Connect discovery document and no\n  API-key console on any institution host probed, so no scopes/ artifact is emitted.\nsummary:\n  types:\n  - none\n  - saml2\nschemes:\n\
  - name: anonymous-read\n  type: none\n  description: >-\n    Public read access with no credential of any kind. GET\n    https://fdat.uni-tuebingen.de/api/records?size=1 returns 200 application/json (437 records);\n    GET https://fdat.uni-tuebingen.de/api/records/zvknn-g0x34 returns 200 with ETag \"6\" and a\n    Link rel=\"linkset\" header; GET https://fdat.uni-tuebingen.de/api/communities?size=1 and\n    /api/vocabularies/languages?size=1 both return 200. Both OAI-PMH providers answer\n    verb=Identify with 200 text/xml unauthenticated. Server-side throttling is advertised rather\n    than authentication — X-RateLimit-Limit: 500, X-RateLimit-Remaining, X-RateLimit-Reset and\n    Retry-After: 60 are returned on FDAT API responses. Note that\n    https://fdat.uni-tuebingen.de/robots.txt disallows /api and /search for crawlers with\n    Crawl-delay: 10; the API is open to clients but the operator does not invite bulk crawling.\n  sources:\n  - https://fdat.uni-tuebingen.de/api/records\n\
  \  - https://fdat.uni-tuebingen.de/oai2d?verb=Identify\n  - https://publikationen.uni-tuebingen.de/oai/request?verb=Identify\n- name: shibboleth-saml2-sso\n  type: saml2\n  description: >-\n    Institutional single sign-on through the university's own Shibboleth Identity Provider,\n    entityID https://idp.uni-tuebingen.de/shibboleth, scope uni-tuebingen.de, registered in DFN-AAI\n    since 2009-05-26 and exported to eduGAIN. SSO endpoints: HTTP-POST\n    https://idp.uni-tuebingen.de/idp/profile/SAML2/POST/SSO, HTTP-Redirect\n    https://idp.uni-tuebingen.de/idp/profile/SAML2/Redirect/SSO, SOAP/ECP\n    https://idp.uni-tuebingen.de/idp/profile/SAML2/SOAP/ECP. NameID formats: persistent and\n    transient. A SAML 2.0 AttributeAuthorityDescriptor with a SOAP AttributeService is also\n    published. The entity asserts REFEDS Research & Scholarship support and SIRTFI + SIRTFI2\n    assurance certification, and is a bwIDM member (the Baden-Württemberg federated identity\n    programme). Relying\
  \ parties obtain the signing key and endpoints from federation metadata, not\n    from the university — this is a federated trust surface, not a self-service API credential.\n  sources:\n  - https://mdq.aai.dfn.de/entities/https%3A%2F%2Fidp.uni-tuebingen.de%2Fshibboleth\n  - https://uni-tuebingen.de/en/einrichtungen/zentrum-fuer-datenverarbeitung/dienstleistungen/digitale-identitaet/single-sign-on/\nnegative_probes:\n- url: https://uni-tuebingen.de/.well-known/security.txt\n  status: 404\n- url: https://uni-tuebingen.de/llms.txt\n  status: 404\n- url: https://uni-tuebingen.de/apis.json\n  status: 404\n- url: https://fdat.uni-tuebingen.de/openapi.json\n  status: 404\n- url: https://fdat.uni-tuebingen.de/.well-known/security.txt\n  status: 404\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-tubingen/refs/heads/main/authentication/university-of-tubingen-authentication.yml
summary_line: none/saml2 · 2 schemes
tags:
- Education
- Higher Education
- University
- Germany
- Research
- Research Data
- Research Repository
- Open Access
- OAI-PMH
- Identity Federation
- Library
- DataCite
---
