---
api_key_in: []
api_specs:
- filename: upm-psasir-oai-pmh-openapi.yml
  format: yaml
  label: PSASIR Institutional Repository — OAI-PMH 2.0
  slug: psasir-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upm/refs/heads/main/openapi/upm-psasir-oai-pmh-openapi.yml
- filename: upm-psasir-eprints-rest-openapi.yml
  format: yaml
  label: PSASIR EPrints REST, Export and OpenSearch
  slug: psasir-eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upm/refs/heads/main/openapi/upm-psasir-eprints-rest-openapi.yml
- filename: upm-myagric-oai-pmh-openapi.yml
  format: yaml
  label: MyAgric — Malaysian Agricultural Repository OAI-PMH 2.0
  slug: myagric-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upm/refs/heads/main/openapi/upm-myagric-oai-pmh-openapi.yml
auth_types: []
description: 'How authentication works across Universiti Putra Malaysia''s machine-readable surfaces. The picture is unusually clean for this cohort: the two harvesting surfaces are entirely open and the identity surface is the authentication system itself, published as SAML metadata rather than protected by it. There is no API key, no OAuth authorization server, no developer registration, and no self-service credential of any kind — because there is no developer programme. Everything an outside consumer can reach, they can reach anonymously.'
kind: authentication
layout: security
method: probed
name: Upm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Universiti Putra Malaysia declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Universiti Putra Malaysia
provider_slug: upm
scheme_count: 0
schemes: []
slug: upm-authentication
source_filename: upm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: Universiti Putra Malaysia\nproviderId: upm\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Unauthenticated live probes of every UPM surface recorded in apis.yml on 2026-09-01. No\n  credentials of any kind were used, and none were needed for any surface listed as public here.\ndescription: >-\n  How authentication works across Universiti Putra Malaysia's machine-readable surfaces. The\n  picture is unusually clean for this cohort: the two harvesting surfaces are entirely open and\n  the identity surface is the authentication system itself, published as SAML metadata rather\n  than protected by it. There is no API key, no OAuth authorization server, no developer\n  registration, and no self-service credential of any kind — because there is no developer\n  programme. Everything an outside consumer can reach, they can reach anonymously.\n\nsurfaces:\n\n  - aid: upm:psasir-oai-pmh\n   \
  \ name: PSASIR OAI-PMH\n    auth: none\n    x-operator: institution\n    detail: >-\n      Fully open. Identify, ListMetadataFormats, ListSets, ListIdentifiers and GetRecord all\n      answered HTTP 200 with no credentials on 2026-09-01. OAI-PMH has no authentication model.\n    evidence:\n      - url: http://psasir.upm.edu.my/cgi/oai2?verb=Identify\n        status: 200\n    transport:\n      https: false\n      note: >-\n        psasir.upm.edu.my does not serve HTTPS. Harvesting is anonymous and the payload is public\n        bibliographic metadata, so there is no credential to expose, but the channel is\n        unauthenticated and unencrypted and integrity of the harvested metadata cannot be assured\n        in transit.\n\n  - aid: upm:psasir-eprints-rest\n    name: PSASIR EPrints REST, export and search\n    auth: none\n    x-operator: institution\n    detail: >-\n      Read access to /rest/, /rest/eprint/{id}.xml, /cgi/export/eprint/{id}/{format}/ and\n      /cgi/search is anonymous.\
  \ EPrints supports HTTP Basic authentication for write operations\n      against the REST datasets; no write was attempted and none is documented for public use.\n      Only public, archived records are exposed — documents whose full_text_status is not\n      `public` are not served.\n    evidence:\n      - url: http://psasir.upm.edu.my/rest/eprint/813.xml\n        status: 200\n      - url: http://psasir.upm.edu.my/cgi/export/eprint/813/JSON/psasir-eprint-813.js\n        status: 200\n    transport:\n      https: false\n\n  - aid: upm:myagric-oai-pmh\n    name: MyAgric OAI-PMH\n    auth: none\n    x-operator: institution\n    detail: Fully open, same EPrints configuration as PSASIR.\n    evidence:\n      - url: http://myagric.upm.edu.my/cgi/oai2?verb=Identify\n        status: 200\n    transport:\n      https: false\n\n  - aid: upm:saml-idp\n    name: UPM Shibboleth SAML 2.0 Identity Provider\n    auth: saml2\n    x-operator: institution\n    detail: >-\n      This surface IS the authentication\
  \ system. The metadata document at the entityID is served\n      anonymously — that is required, it is how relying parties consume it — while the SSO and\n      SLO endpoints behind it perform SAML 2.0 authentication for UPM-ID holders. Federated\n      access is governed by SIFULAN and eduGAIN membership, not by any self-service registration.\n      An outside developer cannot obtain UPM credentials; a federated service provider obtains\n      access by joining the federation.\n    mechanisms:\n      - urn:oasis:names:tc:SAML:2.0:protocol\n      - urn:oasis:names:tc:SAML:1.1:protocol\n      - urn:mace:shibboleth:1.0\n    scope: upm.edu.my\n    evidence:\n      - url: https://idf.upm.edu.my/idp/shibboleth\n        status: 200\n    transport:\n      https: true\n      tls_certificate_subject: CN=idf.upm.edu.my\n\nnot_available:\n  - mechanism: api_key\n    detail: No API key issuance, developer registration or key-management surface was found.\n  - mechanism: oauth2\n    detail: >-\n  \
  \    No OAuth 2.0 authorization server, no /.well-known/oauth-authorization-server and no\n      /.well-known/openid-configuration were found on any UPM host probed.\n  - mechanism: protected_resource_metadata\n    detail: No RFC 9728 protected-resource metadata document exists on any UPM host.\n  - mechanism: dynamic_client_registration\n    detail: No RFC 7591 dynamic client registration endpoint exists.\n\ngated_systems:\n  detail: >-\n    UPM's student, staff and administrative applications — the Putra portal, SMP, the study\n    portal, PutraBLAST — sit behind UPM-ID single sign-on and publish no public interface\n    documentation. They are recorded here as gated rather than as APIs, because no public\n    contract for them was found and none is claimed.\n  evidence:\n    - url: https://sso.upm.edu.my/\n      status: 200\n      note: Answers, but serves a 239-byte redirect stub; no public interface documentation.\n    - url: https://smp.upm.edu.my/\n      status: 200\n      note:\
  \ Answers with a 320-byte stub; login-gated.\n    - url: https://putra.upm.edu.my/\n      status: 200\n      note: Answers with a 1,924-byte stub; login-gated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upm/refs/heads/main/authentication/upm-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Malaysia
- Public Research University
- Research Data
- Institutional Repository
- Open Access
- OAI-PMH
- Identity Federation
- Shibboleth
- Agriculture
- Scholarly Publishing
---
