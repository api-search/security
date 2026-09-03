---
api_key_in: []
api_specs:
- filename: university-of-lisbon-fenixedu-academic-api-openapi.yml
  format: yaml
  label: FenixEdu Academic API (Instituto Superior Tecnico)
  slug: fenixedu-tecnico
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-fenixedu-academic-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Lisbon Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Lisbon declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Lisbon
provider_slug: university-of-lisbon
scheme_count: 0
schemes: []
slug: university-of-lisbon-authentication
source_filename: university-of-lisbon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: University of Lisbon — Authentication\ngenerated: '2026-09-01'\nmethod: probed\nsource:\n  - https://fenix.tecnico.ulisboa.pt/oauth/userdialog\n  - https://fenix.tecnico.ulisboa.pt/oauth/access_token\n  - https://fenix.tecnico.ulisboa.pt/api/fenix/v1/person\n  - https://id.ulisboa.pt/nidp/saml2/metadata\n  - https://repositorio.ulisboa.pt/server/api\nnote: >-\n  Written by API Evangelist from live probes on 2026-09-01. Universidade de Lisboa\n  publishes no consolidated authentication document.\nsurfaces:\n  - surface: FenixEdu Academic API (Instituto Superior Tecnico)\n    x-operator: institution\n    anonymous_access: true\n    anonymous_scope: >-\n      Institution metadata, academic terms, contacts, the degree and course catalog,\n      campus spaces and blueprints, parking, canteen, shuttle and the serialized\n      domain model are all readable with no credential. Probed 2026-09-01: GET /about,\n      /academicterms, /degrees, /degrees/{id}, /spaces, /spaces/{id},\
  \ /parking,\n      /contacts, /domainModel all returned 200 with no Authorization header.\n    scheme: OAuth 2.0 authorization code\n    implementation: Bennu OAuth, copyright Instituto Superior Tecnico, shipped with FenixEdu\n    authorization_url: https://fenix.tecnico.ulisboa.pt/oauth/userdialog\n    token_url: https://fenix.tecnico.ulisboa.pt/oauth/access_token\n    evidence:\n      - url: https://fenix.tecnico.ulisboa.pt/oauth/userdialog\n        status: 200\n        note: Returns the Bennu OAuth consent dialog carrying an Instituto Superior Tecnico copyright header.\n      - url: https://fenix.tecnico.ulisboa.pt/oauth/access_token\n        status: 405\n        note: Method Not Allowed on GET — the token endpoint exists and accepts POST only.\n      - url: https://fenix.tecnico.ulisboa.pt/api/fenix/v1/person\n        status: 401\n        note: 'Unauthenticated call returns {\"error\":\"accessTokenInvalidFormat\"}.'\n    onboarding: >-\n      Application registration requires an authenticated\
  \ Instituto Superior Tecnico\n      account. There is no self-service developer signup open to the public, and no\n      published application-review or rate-limit policy.\n    token_transport: Bearer access token\n    scopes_published: false\n    scopes_note: >-\n      Access scopes are chosen per registered application inside FenixEdu rather than\n      enumerated in any machine-readable or public document. No scope names are\n      asserted here — see scopes/university-of-lisbon-scopes.yml.\n  - surface: Universidade de Lisboa SAML 2.0 identity provider\n    x-operator: institution\n    scheme: SAML 2.0 Web Browser SSO\n    entity_id: https://id.ulisboa.pt/nidp/saml2/metadata\n    metadata_url: https://id.ulisboa.pt/nidp/saml2/metadata\n    federation: RCTSaai (FCCN), published onward to eduGAIN\n    bindings:\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    name_id_formats:\n      - urn:oasis:names:tc:SAML:2.0:nameid-format:persistent\n\
  \      - urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n    roles: [IDPSSODescriptor, SPSSODescriptor, AttributeAuthorityDescriptor]\n    scope: ulisboa.pt\n    evidence:\n      - url: https://id.ulisboa.pt/nidp/saml2/metadata\n        status: 200\n        note: >-\n          Live SAML 2.0 EntityDescriptor. OrganizationName \"Universidade de Lisboa\",\n          OrganizationURL www.ulisboa.pt.\n  - surface: Instituto Superior Tecnico SAML 2.0 identity provider\n    x-operator: institution\n    scheme: SAML 2.0 Web Browser SSO\n    entity_id: https://id.tecnico.ulisboa.pt/saml\n    federation: RCTSaai (FCCN), published onward to eduGAIN\n    scope: tecnico.ulisboa.pt\n    assurance: SIRTFI asserted in the eduGAIN registry record\n    evidence:\n      - url: https://technical.edugain.org/api.php?action=list_entities&format=json\n        status: 200\n        note: >-\n          eduGAIN entity 673215, IDPSSODescriptor, registration authority\n          https://www.fccn.pt, first seen\
  \ 2018-01-30, eccs_status 1, sirtfi_status 1.\n    caveat: >-\n      The entityID is an identifier, not a dereferenceable endpoint; GET on it returns\n      404 from nginx. Metadata is distributed through the RCTSaai and eduGAIN\n      aggregates, not from this URL.\n  - surface: Repositorio ULisboa (DSpace 7.6.1)\n    x-operator: institution\n    anonymous_access: true\n    anonymous_scope: >-\n      The full REST and OAI-PMH read surface is anonymous. Probed 2026-09-01:\n      GET /server/api and GET /server/api/core/communities both 200.\n    scheme: Session token plus OIDC/SAML login for deposit and administration\n    evidence:\n      - url: https://repositorio.ulisboa.pt/server/api\n        status: 200\n        note: HAL root advertises authn, authorizations, oidc and groups endpoints.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/authentication/university-of-lisbon-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Portugal
- Europe
- Public Research University
- Course Catalog
- Research Repository
- Library
- Identity Federation
- OAI-PMH
- Open Access
- Erasmus Without Paper
- Metadata
---
