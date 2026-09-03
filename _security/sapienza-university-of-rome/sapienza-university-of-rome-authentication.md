---
api_key_in: []
auth_types:
- none
- http-basic
- saml
description: ''
kind: authentication
layout: security
method: probed
name: Sapienza University Of Rome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sapienza University of Rome secures its APIs with none, http-basic, and saml across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sapienza University of Rome
provider_slug: sapienza-university-of-rome
scheme_count: 4
schemes:
- description: Both OAI-PMH 2.0 providers are keyless and anonymous. No Authorization header, API key, referer or cookie is required for any verb.
  evidence:
  - status: 200
    url: https://iris.uniroma1.it/oai/request?verb=Identify
  - status: 200
    url: https://iris.uniroma1.it/oai/request?verb=ListRecords&metadataPrefix=oai_dc
  - status: 200
    url: https://rosa.uniroma1.it/rosa04/index/oai?verb=Identify
  - status: 200
    url: https://rosa.uniroma1.it/rosa04/index/oai?verb=ListSets
  name: oai-pmh-anonymous
  operator: institution
  status: open
  type: none
- description: The DSpace REST API on the IRIS host rejects anonymous callers with HTTP basic authentication. The response body is the literal string "HTTP Status 401 - Invalid basic authentication token" (53 bytes, no WWW-Authenticate challenge document, no JSON error envelope). No public route to obtain credentials is documented anywhere on uniroma1.it; the platform is DSpace-CRIS supplied by CINECA, so both the scheme and the contract are the vendor's.
  evidence:
  - status: 401
    url: https://iris.uniroma1.it/rest/
  - status: 401
    url: https://iris.uniroma1.it/rest/items
  name: iris-dspace-rest-basic
  operator: institution
  scheme: basic
  status: gated
  type: http
- description: The Open Journal Systems REST API v1 on the R.O.SA host answers anonymous callers with 403 application/json {"error":"api.403.unauthorized","errorMessage":"You are not authorized to access the requested resource."}. OJS gates /api/v1/ behind a per-user API token issued from the journal editorial back office; there is no public registration flow. The API contract is PKP's, not Sapienza's, and is not saved under this institution.
  evidence:
  - status: 403
    url: https://rosa.uniroma1.it/rosa04/annali_di_botanica/api/v1/issues
  name: ojs-rest-api-token
  operator: institution
  status: gated
  type: apiKey
- description: Human access to Sapienza's gated systems is federated through the institution's own Shibboleth SAML 2.0 identity provider, entityID https://idp.uniroma1.it/idp/shibboleth, scope "uniroma1.it", registered in the IDEM GARR AAI national federation. The IdP metadata is machine-readable and public; the authentication itself is interactive and not an API surface.
  evidence:
  - status: 200
    url: https://idp.uniroma1.it/idp/shibboleth
  - status: 200
    url: https://md.idem.garr.it/metadata/idem-metadata-sha256.xml
  name: shibboleth-saml-sso
  operator: institution
  status: federated
  type: saml
slug: sapienza-university-of-rome-authentication
source_filename: sapienza-university-of-rome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes of Sapienza University of Rome institution-operated hosts on 2026-09-01. No OpenAPI\n  or published security scheme exists for any Sapienza surface; every entry below is the observed\n  behaviour of a real request, recorded so an unauthenticated 401/403 is not mistaken for an\n  absent API or for a callable one.\nnote: >-\n  Sapienza publishes no developer portal, no self-service key issuance and no authentication\n  documentation. Two REST APIs exist on institution hosts and both refuse anonymous callers; two\n  OAI-PMH providers on the same hosts are fully open and keyless. This split — an open harvesting\n  protocol beside a closed product REST API — is the whole of the institution's public access\n  story.\nsummary:\n  types:\n  - none\n  - http-basic\n  - saml\n  keyless_surfaces: 2\n  gated_surfaces: 2\n  self_service_key_issuance: false\n  documented: false\nschemes:\n- name: oai-pmh-anonymous\n  type:\
  \ none\n  status: open\n  operator: institution\n  description: >-\n    Both OAI-PMH 2.0 providers are keyless and anonymous. No Authorization header, API key,\n    referer or cookie is required for any verb.\n  evidence:\n  - url: https://iris.uniroma1.it/oai/request?verb=Identify\n    status: 200\n  - url: https://iris.uniroma1.it/oai/request?verb=ListRecords&metadataPrefix=oai_dc\n    status: 200\n  - url: https://rosa.uniroma1.it/rosa04/index/oai?verb=Identify\n    status: 200\n  - url: https://rosa.uniroma1.it/rosa04/index/oai?verb=ListSets\n    status: 200\n- name: iris-dspace-rest-basic\n  type: http\n  scheme: basic\n  status: gated\n  operator: institution\n  description: >-\n    The DSpace REST API on the IRIS host rejects anonymous callers with HTTP basic authentication.\n    The response body is the literal string \"HTTP Status 401 - Invalid basic authentication token\"\n    (53 bytes, no WWW-Authenticate challenge document, no JSON error envelope). No public route to\n   \
  \ obtain credentials is documented anywhere on uniroma1.it; the platform is DSpace-CRIS supplied\n    by CINECA, so both the scheme and the contract are the vendor's.\n  evidence:\n  - url: https://iris.uniroma1.it/rest/\n    status: 401\n  - url: https://iris.uniroma1.it/rest/items\n    status: 401\n- name: ojs-rest-api-token\n  type: apiKey\n  status: gated\n  operator: institution\n  description: >-\n    The Open Journal Systems REST API v1 on the R.O.SA host answers anonymous callers with 403\n    application/json {\"error\":\"api.403.unauthorized\",\"errorMessage\":\"You are not authorized to\n    access the requested resource.\"}. OJS gates /api/v1/ behind a per-user API token issued from\n    the journal editorial back office; there is no public registration flow. The API contract is\n    PKP's, not Sapienza's, and is not saved under this institution.\n  evidence:\n  - url: https://rosa.uniroma1.it/rosa04/annali_di_botanica/api/v1/issues\n    status: 403\n- name: shibboleth-saml-sso\n\
  \  type: saml\n  status: federated\n  operator: institution\n  description: >-\n    Human access to Sapienza's gated systems is federated through the institution's own Shibboleth\n    SAML 2.0 identity provider, entityID https://idp.uniroma1.it/idp/shibboleth, scope\n    \"uniroma1.it\", registered in the IDEM GARR AAI national federation. The IdP metadata is\n    machine-readable and public; the authentication itself is interactive and not an API surface.\n  evidence:\n  - url: https://idp.uniroma1.it/idp/shibboleth\n    status: 200\n  - url: https://md.idem.garr.it/metadata/idem-metadata-sha256.xml\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sapienza-university-of-rome/refs/heads/main/authentication/sapienza-university-of-rome-authentication.yml
summary_line: none/http-basic/saml · 4 schemes
tags:
- Education
- Higher Education
- University
- Italy
- Research
- Research Repository
- Open Access
- Open Data
- Library
- OAI-PMH
- Identity Federation
- Scholarly Publishing
---
