---
api_key_in: []
api_specs:
- filename: tu-delft-account-api-openapi.yml
  format: yaml
  label: Delft University of Technology Account API
  slug: tu-delft-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-delft/refs/heads/main/openapi/tu-delft-account-api-openapi.yml
- filename: tu-delft-collections-api-openapi.yml
  format: yaml
  label: Delft University of Technology Collections API
  slug: tu-delft-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-delft/refs/heads/main/openapi/tu-delft-collections-api-openapi.yml
- filename: tu-delft-datasets-api-openapi.yml
  format: yaml
  label: Delft University of Technology Datasets API
  slug: tu-delft-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-delft/refs/heads/main/openapi/tu-delft-datasets-api-openapi.yml
- filename: tu-delft-reference-api-openapi.yml
  format: yaml
  label: Delft University of Technology Reference API
  slug: tu-delft-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-delft/refs/heads/main/openapi/tu-delft-reference-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Tu Delft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delft University of Technology declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Delft University of Technology
provider_slug: tu-delft
scheme_count: 0
schemes: []
slug: tu-delft-authentication
source_filename: tu-delft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-19 of https://data.4tu.nl/v2/account/articles (HTTP 403\n  InvalidSessionToken), https://login.tudelft.nl/ (HTTP 200),\n  https://login.tudelft.nl/sso/saml2/idp/metadata.php (HTTP 200,\n  application/samlmetadata+xml), https://metadata.surfconext.nl/idps-metadata.xml (HTTP 200),\n  https://pure.tudelft.nl/ws/oai?verb=Identify (HTTP 401), plus\n  https://raw.githubusercontent.com/4TUResearchData/djehuty/main/docs/api.md and\n  https://www.tudelft.nl/en/it-manuals/netid (HTTP 200).\nnote: >-\n  TU Delft has two entirely separate authentication stories and they should not be conflated.\n  Human access to institutional services runs through NetID over SAML 2.0, federated nationally\n  through SURFconext and onward to eduGAIN. Machine access to the one public API the institution\n  operates (4TU.ResearchData) uses a personal bearer token issued from a dashboard, with no\n  OAuth 2.0, no OIDC discovery\
  \ document and no published scope vocabulary. The legacy\n  api.tudelft.nl OAuth 2.0 authorization service at oauth.tudelft.nl no longer answers on\n  either port 80 or 443 from the public internet.\nmechanisms:\n  - id: api-token\n    name: djehuty personal API token\n    applies_to: 4TU.ResearchData API (data.4tu.nl)\n    x-operator: institution\n    type: bearer\n    scheme: token\n    header: 'Authorization: token YOUR_TOKEN_HERE'\n    issuance: Self-service from the depositor dashboard after NetID/ORCID/SRAM login.\n    public_read: true\n    evidence: >-\n      GET /v2/account/articles without a token returns HTTP 403\n      {\"message\":\"Invalid or unknown session token\",\"code\":\"InvalidSessionToken\"}.\n      All /v2 and /v3 read endpoints listed in openapi/ answered HTTP 200 with no credentials.\n    oauth2: false\n    oidc: false\n    scopes_published: false\n  - id: saml-idp\n    name: TU Delft SAML 2.0 Identity Provider (NetID)\n    applies_to: Institutional web services,\
  \ SURFconext service providers, eduGAIN\n    x-operator: institution\n    type: saml2\n    entity_id: https://login.tudelft.nl/sso/saml2/idp/metadata.php\n    metadata_url: https://login.tudelft.nl/sso/saml2/idp/metadata.php\n    software: SimpleSAMLphp\n    federation: SURFconext (SURF, Netherlands) -> eduGAIN\n    federation_metadata: https://metadata.surfconext.nl/idps-metadata.xml\n    display_names: ['Technische Universiteit Delft', 'Delft University of Technology']\n    evidence: >-\n      The entity is present in the live SURFconext IdP aggregate with a SingleSignOnService\n      HTTP-Redirect binding at\n      https://engine.surfconext.nl/authentication/idp/single-sign-on/key:20230503/a2f60e8691e4518b7cb67605ecd88a8d,\n      and the institution's own metadata document is served directly from login.tudelft.nl.\n    local_copy: authentication/tu-delft-saml-idp-metadata.xml\n  - id: sram\n    name: SURF Research Access Management (SRAM) collaboration\n    applies_to: 4TU.ResearchData\
  \ depositor onboarding\n    x-operator: tenant\n    type: saml2-broker\n    evidence: >-\n      djehuty's configuration documentation describes joining an SRAM collaboration to grant\n      access to a djehuty instance (organization-api-token + collaboration-id). SRAM is\n      operated by SURF, not by TU Delft.\n  - id: orcid\n    name: ORCID as identity provider\n    applies_to: 4TU.ResearchData depositor login and author records\n    x-operator: vendor\n    type: oauth2\n    evidence: >-\n      djehuty documents ORCID both as a primary login identity provider and as a way to couple\n      an author record to an ORCID iD. ORCID is operated by ORCID, Inc.\n  - id: pure-ws\n    name: Elsevier Pure Web Service\n    applies_to: pure.tudelft.nl / research.tudelft.nl\n    x-operator: tenant\n    type: api-key\n    evidence: >-\n      https://pure.tudelft.nl/ws/oai?verb=Identify returns HTTP 401 — the interface exists and\n      is gated, not absent. The API documentation served under pure.tudelft.nl/ws/api/\
  \ carries\n      rel=canonical to https://api.elsevierpure.com/ws/api/index.html, which is the ownership\n      signal: the contract is Elsevier's, the tenancy is TU Delft's.\n  - id: legacy-oauth\n    name: api.tudelft.nl OAuth 2.0 authorization service (retired)\n    applies_to: The former TU Delft institutional API platform\n    x-operator: institution\n    type: oauth2\n    status: unreachable\n    evidence: >-\n      api.tudelft.nl resolves to 131.180.187.26 and oauth.tudelft.nl to 131.180.187.27, both\n      inside TU Delft's DUNET netblock, but TCP connections to ports 80 and 443 time out from\n      the public internet. apidoc.tudelft.nl has no DNS record at all. The OAuth 2.0\n      developer's guide previously published at api.tudelft.nl/cms/developers-guide/oauth2/\n      is not retrievable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-delft/refs/heads/main/authentication/tu-delft-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Technical University
- Research Data
- Open Access
- Identity Federation
- Research Repository
- Research Computing
- 4TU.Federation
- Netherlands
- Europe
---
