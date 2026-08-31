---
api_key_in: []
api_specs:
- filename: university-of-bristol-research-portal-oai-pmh-openapi.yml
  format: yaml
  label: University of Bristol Research Portal OAI-PMH
  slug: research-portal-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/openapi/university-of-bristol-research-portal-oai-pmh-openapi.yml
auth_types:
- none
- apiKey
- saml
description: ''
kind: authentication
layout: security
method: probed
name: University Of Bristol Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Bristol secures its APIs with none, apiKey, and saml across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Bristol
provider_slug: university-of-bristol
scheme_count: 0
schemes: []
slug: university-of-bristol-authentication
source_filename: university-of-bristol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live unauthenticated probes of University of Bristol hosts on 2026-08-30\nnote: >-\n  REPLACES the 2026-07-11 version of this file, which was derived from\n  openapi/university-of-bristol-pure-research-api.yaml — a hand-authored subset of Elsevier's Pure\n  product contract that has been removed from this repository as vendor-operated. Authentication is\n  now recorded per surface, with the operator of each surface named.\nsummary:\n  types:\n    - none\n    - apiKey\n    - saml\n  institution_operated_keyless_surfaces: 2\nsurfaces:\n  - id: research-portal-oai-pmh\n    x-operator: institution\n    endpoint: https://research-information.bris.ac.uk/ws/oai\n    scheme: none\n    detail: >-\n      No API key, token, cookie or affiliation is required. Every OAI-PMH verb tested on 2026-08-30\n      executed anonymously; five returned well-formed OAI-PMH 2.0 XML and Identify returned HTTP 500.\n    evidence:\n      - url: https://research-information.bris.ac.uk/ws/oai?verb=ListRecords&metadataPrefix=oai_dc\n\
  \        status: 200\n        detail: 100 records returned with no credential presented.\n  - id: idp-shibboleth-metadata\n    x-operator: institution\n    endpoint: https://idp.bris.ac.uk/idp/shibboleth\n    scheme: none\n    detail: >-\n      SAML 2.0 IdP metadata is served anonymously. The identity service itself is of course\n      credential-gated; the METADATA describing it is public, which is what makes it a\n      machine-readable surface.\n    evidence:\n      - url: https://idp.bris.ac.uk/idp/shibboleth\n        status: 200\n        detail: 5,990 bytes of application/xml SAML 2.0 metadata, no credential presented.\n  - id: idp-shibboleth-sso\n    x-operator: institution\n    endpoint: https://idp.bris.ac.uk/idp/profile/SAML2/Redirect/SSO\n    scheme: saml\n    detail: >-\n      SAML 2.0 web browser SSO. Bindings observed in the live metadata: Shibboleth/SSO,\n      SAML2/POST/SSO, SAML2/POST-SimpleSign/SSO, SAML2/Redirect/SSO. Trust is established through\n      the UK Access\
  \ Management Federation, not through a self-serve credential; scope bris.ac.uk;\n      REFEDS Research & Scholarship entity category asserted.\n  - id: data-bris-research-data-repository\n    x-operator: institution\n    endpoint: https://data.bris.ac.uk/datasets/\n    scheme: none\n    detail: >-\n      Open dataset payload index served without credentials. Individual datasets may carry their own\n      access conditions; the index itself answered anonymously (200, 315,475 bytes).\ntenant_surfaces:\n  - id: pure-web-services\n    x-operator: tenant\n    endpoint: https://research-information.bris.ac.uk/ws/api\n    scheme: apiKey\n    detail: >-\n      Elsevier Pure Web Services running under the institution's host. api-key gated; no key is\n      issued self-serve. Verified 2026-08-30: GET /ws/api/524/research-outputs returned 401 with no\n      key. The OpenAPI describing it is Elsevier's product contract\n      (info.title \"Pure API\", info.contact.email pure-support@elsevier.com,\
  \ 826 paths) and is\n      deliberately NOT stored in this repository.\n    evidence:\n      - url: https://research-information.bris.ac.uk/ws/api/524/research-outputs\n        status: 401\n      - url: https://research-information.bris.ac.uk/ws/api/openapi.json\n        status: 200\n        detail: The vendor's own contract, publicly readable, 1,740,065 bytes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/authentication/university-of-bristol-authentication.yml
summary_line: none/apiKey/saml · 0 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Research Repository
- Metadata Harvesting
- OAI-PMH
- Identity Federation
- Open Data
---
