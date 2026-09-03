---
api_key_in: []
api_specs:
- filename: university-of-minnesota-gems-exchange-soil-openapi.yml
  format: yaml
  label: GEMS Informatics Exchange APIs
  slug: gems-exchange-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-minnesota/refs/heads/main/openapi/university-of-minnesota-gems-exchange-soil-openapi.yml
- filename: university-of-minnesota-umedia-openapi.yml
  format: yaml
  label: UMedia Digital Collections JSON API
  slug: umedia-digital-collections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-minnesota/refs/heads/main/openapi/university-of-minnesota-umedia-openapi.yml
auth_types: []
description: How each University of Minnesota surface authenticates. Recorded per surface because the institution operates several unrelated surfaces with unrelated auth models, and two of them are run on vendor platforms under a UMN tenancy rather than by the University itself.
kind: authentication
layout: security
method: probed
name: University Of Minnesota Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Minnesota declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Minnesota
provider_slug: university-of-minnesota
scheme_count: 0
schemes: []
slug: university-of-minnesota-authentication
source_filename: university-of-minnesota-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: University of Minnesota — authentication across programmable surfaces\ndescription: >-\n  How each University of Minnesota surface authenticates. Recorded per surface because the\n  institution operates several unrelated surfaces with unrelated auth models, and two of them are\n  run on vendor platforms under a UMN tenancy rather than by the University itself.\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of exchange-1.gems.msi.umn.edu, umedia.lib.umn.edu,\n  conservancy.umn.edu, integration-boomi.umn.edu and umn-prod-apigw.boomi.cloud, plus the\n  University's own documentation on sites.google.com/umn.edu/integration-apis and the\n  GEMS-UMN/Exchange-Notebooks repository.\nsurfaces:\n  - surface: GEMS Informatics Exchange APIs\n    x-operator: institution\n    host: exchange-1.gems.msi.umn.edu\n    scheme: api-key\n    location: header\n    parameter: apikey\n    declared_in_contract: false\n    evidence:\n      - url: https://exchange-1.gems.msi.umn.edu/soil/v2/datasets\n\
  \        status: 401\n        body: '{\"message\":\"Missing API key in request\"}'\n        note: >-\n          Every data path returns 401 without a key. The OpenAPI documents themselves declare NO\n          components.securitySchemes and NO top-level security[], so the requirement is real but\n          undeclared in the contract — a gap worth reporting back to GEMS.\n      - url: https://github.com/GEMS-UMN/Exchange-Notebooks\n        status: 200\n        note: >-\n          The University's own example notebooks set the credential with\n          `s.headers.update({'apikey': key})`, which is where the header name is evidenced.\n    key_issuance: https://exchange-1.gems.msi.umn.edu/portal/home\n    key_issuance_status: 200\n    openapi_public_without_key: true\n    exception:\n      path: /weather/v2/openapi.json\n      status: 401\n      note: The weather API requires a key even to read its OpenAPI document; the other nine do not.\n  - surface: UMedia Digital Collections JSON API\n\
  \    x-operator: institution\n    host: umedia.lib.umn.edu\n    scheme: none\n    declared_in_contract: false\n    evidence:\n      - url: https://umedia.lib.umn.edu/search.json?q=test\n        status: 200\n        note: Anonymous read succeeds. No key, no token, no session.\n      - url: https://umedia.lib.umn.edu/\n        status: 403\n        note: >-\n          The HTML site sits behind an Azure WAF that 403s a default curl User-Agent while the\n          .json paths answer. This is a bot challenge, not a dead host — the surface grades LIVE.\n  - surface: UMN Digital Conservancy / DRUM (DSpace 10.0 REST + OAI-PMH)\n    x-operator: institution\n    host: conservancy.umn.edu\n    scheme: mixed\n    detail: >-\n      Discovery endpoints are anonymous; item-level endpoints require authentication. The REST\n      contract is DSpace's generic product contract, not a University-authored one.\n    evidence:\n      - url: https://conservancy.umn.edu/server/api\n        status: 200\n       \
  \ note: DSpace 10.0 HAL root, anonymous.\n      - url: https://conservancy.umn.edu/server/api/core/communities?size=2\n        status: 200\n        note: Community listing, anonymous.\n      - url: https://conservancy.umn.edu/server/api/core/items?size=1\n        status: 401\n        body: '{\"status\":401,\"error\":\"Unauthorized\",\"message\":\"Authentication is required\"}'\n      - url: https://conservancy.umn.edu/server/oai/request?verb=Identify\n        status: 200\n        note: OAI-PMH 2.0, anonymous, no credential of any kind.\n  - surface: Common Good APIs (OIT Integrations)\n    x-operator: institution\n    host: integration-boomi.umn.edu\n    scheme: gated\n    detail: >-\n      Access is granted by request and data-custodian approval, scaled to the University's data\n      classification tiers (public / private / restricted / highly restricted). No anonymous\n      credential path exists and the Swagger documents live only inside the tenant developer\n      portal, behind\
  \ its sign-in.\n    evidence:\n      - url: https://sites.google.com/umn.edu/integration-apis/common-good-apis\n        status: 200\n      - url: https://umn-prod-apigw.boomi.cloud:18077/#catalog\n        status: 200\n        note: >-\n          The catalog UI answers, but it is a GWT single-page app; no anonymous REST or Swagger\n          path was reachable. /api/{id}/swagger, /api/{id}/openapi, /rest/apis and eleven other\n          candidate paths all returned 404.\n  - surface: Institutional identity (Shibboleth IdP)\n    x-operator: federation\n    host: login.umn.edu\n    scheme: saml2\n    detail: >-\n      The University operates its own Shibboleth IdP and publishes it through InCommon. This is\n      the auth surface behind almost every gated University application.\n    evidence:\n      - url: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aumn.edu\n        status: 200\n        note: >-\n          entityID urn:mace:incommon:umn.edu, shibmd:Scope umn.edu, SingleSignOnService\
  \ at\n          https://login.umn.edu/idp/profile/SAML2/Redirect/SSO.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-minnesota/refs/heads/main/authentication/university-of-minnesota-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- United States
- Minnesota
- Big Ten
- Land Grant
- Public Research University
- Research Data
- Research Repository
- Open Data
- Geospatial
- Agriculture
- Climate
- Digital Collections
- Identity Federation
- Research Computing
---
