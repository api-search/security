---
api_key_in: []
api_specs:
- filename: ntu-search-api-openapi.yml
  format: yaml
  label: DR-NTU (Data) — Dataverse API
  slug: ntu-drntu-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-search-api-openapi.yml
- filename: ntu-discover-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Discover API
  slug: ntu-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-discover-api-openapi.yml
- filename: ntu-items-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Items API
  slug: ntu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-items-api-openapi.yml
- filename: ntu-oai-pmh-api-openapi.yml
  format: yaml
  label: Nanyang Technological University OAI PMH API
  slug: ntu-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-oai-pmh-api-openapi.yml
- filename: ntu-root-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Root API
  slug: ntu-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-root-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Ntu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nanyang Technological University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Nanyang Technological University
provider_slug: ntu
scheme_count: 0
schemes: []
slug: ntu-authentication
source_filename: ntu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# ntu — authentication posture across NTU's programmable surfaces.\ngenerated: '2026-08-19'\nmethod: probed\nsource: live probes 2026-08-19; https://libguides.ntu.edu.sg/drntudataguidespolicies/APITermsOfUse\nprovider: ntu\nauthentication:\n\n  - surface: DR-NTU (Data) — Dataverse REST API\n    x-operator: institution\n    baseURL: https://researchdata.ntu.edu.sg/api\n    public_read: true\n    scheme: none\n    detail: >-\n      Dataverse serves published search and version endpoints unauthenticated. Deposit,\n      administration and access to restricted files require a Dataverse API token supplied in the\n      X-Dataverse-key header. Only the unauthenticated read subset is described in openapi/.\n    token_header: X-Dataverse-key\n    token_issuance: NTU account, via the DR-NTU (Data) web UI. Not self-service for non-NTU users.\n    verified: false\n    verification_note: >-\n      Could not be re-verified on 2026-08-19 — the host returns a Citrix bot-management 403 to\
  \ our\n      probes on every path including the site root. Scheme is taken from the archived contract and\n      the Dataverse 6.1 platform documentation, not from a fresh probe.\n\n  - surface: DR-NTU (Digital Repository) — DSpace-CRIS REST API\n    x-operator: tenant\n    baseURL: https://dr.ntu.edu.sg/server/api\n    public_read: true\n    scheme: none\n    detail: >-\n      Discovery and item read operations answer unauthenticated; verified live 2026-08-19\n      (HTTP 200, application/hal+json). Write and restricted-content operations use the DSpace 7\n      JWT bearer flow at /server/api/authn/login. That flow is 4Science's DSpace-CRIS\n      implementation, not NTU engineering.\n    verified: true\n\n  - surface: NTU institutional single sign-on (SGAF / eduGAIN)\n    x-operator: tenant\n    entityID: https://ntu-entra.singaren.net.sg/simplesaml/saml2/idp/metadata.php\n    scheme: SAML 2.0 (IDPSSODescriptor + AttributeAuthorityDescriptor)\n    scope: ntu.edu.sg\n    detail: >-\n\
  \      This is the only NTU-attributed authentication surface that is both machine-readable and\n      independently registered. It authenticates humans into federated services; it is not an API\n      authorization surface for third-party developers.\n    verified: true\n\n  - surface: api.ntu.edu.sg\n    x-operator: institution\n    scheme: unknown\n    detail: >-\n      A live NTU-owned API gateway host that returns a structured JSON envelope\n      ({\"statusCode\":404,\"message\":\"Resource not found\"}) on every path probed. No authentication\n      scheme is discoverable because no route is. Recorded so the host is not mistaken for absent.\n    verified: false\n\nnotes:\n  - >-\n    NTU publishes no developer portal, no API key self-service, and no OAuth or OIDC authorization\n    server for third-party API consumers. Nothing in this file should be read as a developer\n    onboarding path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/authentication/ntu-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Singapore
- Public Research University
- Research Data
- Research Repository
- Identity Federation
- Open Access
- Course Catalog
- Library
- OAI-PMH
---
