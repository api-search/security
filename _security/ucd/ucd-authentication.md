---
api_key_in: []
api_specs:
- filename: ucd-oai-pmh-openapi.yml
  format: yaml
  label: Research Repository UCD — OAI-PMH 2.0
  slug: oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/openapi/ucd-oai-pmh-openapi.yml
auth_types: []
description: How authentication actually works across the surfaces University College Dublin operates. UCD runs no API key programme, no OAuth authorization server and no developer self-service credential of any kind. Its one institution-operated authentication surface is federated SAML 2.0 single sign-on for people, which is not an API credential and cannot be used by an unaffiliated client.
kind: authentication
layout: security
method: probed
name: Ucd Authentication
name_suffix: Authentication
oauth_flows: []
overview: University College Dublin declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: University College Dublin
provider_slug: ucd
scheme_count: 3
schemes:
- audience: Staff, students and federated service providers. Access is granted by institutional affiliation, not by registration; there is no route for an unaffiliated developer or an agent to obtain a credential.
  bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  entityID: https://sso.ucd.ie/idp/shibboleth
  federation: Edugate (HEAnet), connected to eduGAIN
  firstSeenInEduGAIN: '2017-04-13'
  metadata:
    authoritative: The Edugate / eduGAIN federation aggregate. UCD's entity is discoverable via https://technical.edugain.org/entities and in https://mds.edugain.org/edugain-v2.xml.
    warning: Do NOT consume https://sso.ucd.ie/idp/shibboleth as metadata. It returns HTTP 200 with Content-Type application/xml, but the body is the stock Shibboleth IdP example file — entityID "https://idp.exanple.com/idp" (sic), Scope "example.com", endpoint Locations on https://localhost/. Verified 2026-08-30.
  name: EdugateSAML
  operator: institution
  registrationAuthority: http://www.heanet.ie
  role: identity-provider
  scope: ucd.ie
  sirtfi: true
  software: Shibboleth Identity Provider
  type: saml2
- applies:
  - https://researchrepository.ucd.ie/server/oai/request
  - https://researchrepository.ucd.ie/server/oai/openairecris
  - https://digital.ucd.ie/assets/data/metadata.json
  description: The OAI-PMH endpoints and the UCD Digital Library static data exports are anonymous and unauthenticated. All six OAI-PMH verbs answered without a credential on 2026-08-30. No key, no token, no registration, no quota disclosed.
  name: AnonymousHarvest
  operator: institution
  role: public-read
  type: none
- applies:
  - https://researchrepository.ucd.ie/server/api/authn
  - https://researchrepository.ucd.ie/server/api/oidc
  description: The DSpace-CRIS 7.6.1 REST API on the same deployment advertises `authn` and `oidc` link relations. This is DSpace's own authentication contract, shipped by 4Science, on a UCD-branded tenant host (researchrepository.ucd.ie CNAMEs to ucd7.4science.cloud). It is recorded here as an institutional fact and is NOT credited to UCD as an authentication programme of their own.
  name: DSpaceRestAuthn
  operator: tenant
  role: vendor-contract
  type: platform
slug: ucd-authentication
source_filename: ucd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nprovider: University College Dublin\nproviderId: ucd\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-30 of sso.ucd.ie, researchrepository.ucd.ie,\n  digital.ucd.ie and the eduGAIN technical registry. Replaces the 2026-07-11\n  file, which was derived from openapi/ucd-duchas.yaml — a contract operated by\n  the Gaois research group at DCU, not by UCD, and withdrawn by its operator.\ndescription: >-\n  How authentication actually works across the surfaces University College Dublin\n  operates. UCD runs no API key programme, no OAuth authorization server and no\n  developer self-service credential of any kind. Its one institution-operated\n  authentication surface is federated SAML 2.0 single sign-on for people, which\n  is not an API credential and cannot be used by an unaffiliated client.\nschemes:\n\n  - name: EdugateSAML\n    type: saml2\n    role: identity-provider\n    operator: institution\n    entityID: https://sso.ucd.ie/idp/shibboleth\n\
  \    software: Shibboleth Identity Provider\n    federation: Edugate (HEAnet), connected to eduGAIN\n    registrationAuthority: http://www.heanet.ie\n    scope: ucd.ie\n    sirtfi: true\n    firstSeenInEduGAIN: '2017-04-13'\n    metadata:\n      authoritative: >-\n        The Edugate / eduGAIN federation aggregate. UCD's entity is discoverable\n        via https://technical.edugain.org/entities and in\n        https://mds.edugain.org/edugain-v2.xml.\n      warning: >-\n        Do NOT consume https://sso.ucd.ie/idp/shibboleth as metadata. It returns\n        HTTP 200 with Content-Type application/xml, but the body is the stock\n        Shibboleth IdP example file — entityID \"https://idp.exanple.com/idp\"\n        (sic), Scope \"example.com\", endpoint Locations on https://localhost/.\n        Verified 2026-08-30.\n    bindings:\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    audience: >-\n      Staff, students and\
  \ federated service providers. Access is granted by\n      institutional affiliation, not by registration; there is no route for an\n      unaffiliated developer or an agent to obtain a credential.\n\n  - name: AnonymousHarvest\n    type: none\n    role: public-read\n    operator: institution\n    applies:\n      - https://researchrepository.ucd.ie/server/oai/request\n      - https://researchrepository.ucd.ie/server/oai/openairecris\n      - https://digital.ucd.ie/assets/data/metadata.json\n    description: >-\n      The OAI-PMH endpoints and the UCD Digital Library static data exports are\n      anonymous and unauthenticated. All six OAI-PMH verbs answered without a\n      credential on 2026-08-30. No key, no token, no registration, no quota\n      disclosed.\n\n  - name: DSpaceRestAuthn\n    type: platform\n    role: vendor-contract\n    operator: tenant\n    applies:\n      - https://researchrepository.ucd.ie/server/api/authn\n      - https://researchrepository.ucd.ie/server/api/oidc\n\
  \    description: >-\n      The DSpace-CRIS 7.6.1 REST API on the same deployment advertises `authn`\n      and `oidc` link relations. This is DSpace's own authentication contract,\n      shipped by 4Science, on a UCD-branded tenant host\n      (researchrepository.ucd.ie CNAMEs to ucd7.4science.cloud). It is recorded\n      here as an institutional fact and is NOT credited to UCD as an\n      authentication programme of their own.\n\nnotFound:\n  - surface: OAuth 2.0 / OpenID Connect for third parties\n    checked: >-\n      No authorization server, no client registration, no\n      /.well-known/openid-configuration and no\n      /.well-known/oauth-protected-resource on any UCD host.\n  - surface: API keys\n    checked: >-\n      No developer portal, no key issuance page, no rate-limit tiers. UCD\n      operates no API key programme.\n  - surface: .well-known/security.txt\n    checked: https://www.ucd.ie/.well-known/security.txt returned 404 on 2026-08-30.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucd/refs/heads/main/authentication/ucd-authentication.yml
summary_line: 3 schemes
tags:
- University
- Higher Education
- Education
- Ireland
- Europe
- Public Research University
- Research Repository
- Open Access
- OAI-PMH
- Identity Federation
- Cultural Heritage
- Open Data
---
