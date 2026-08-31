---
api_key_in: []
api_specs:
- filename: university-of-copenhagen-curis-oai-pmh-openapi.yml
  format: yaml
  label: University of Copenhagen CURIS OAI-PMH Repository Interface
  slug: curis-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-copenhagen/refs/heads/main/openapi/university-of-copenhagen-curis-oai-pmh-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: University Of Copenhagen Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Copenhagen declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Copenhagen
provider_slug: university-of-copenhagen
scheme_count: 0
schemes: []
slug: university-of-copenhagen-authentication
source_filename: university-of-copenhagen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nx-evidence-method: probed\nx-evidence-note: >-\n  Written by API Evangelist from live HTTP probes of the institution's own endpoints on\n  2026-08-30; every status code and payload quoted below was observed, not inferred. `derived`\n  is the provenance-manifest term for \"we wrote it\" — the provider did not publish this file.\nsource: https://curis.ku.dk/ws/oai\nsummary:\n  types: []\n  note: >-\n    The one institution-operated contract Copenhagen publishes takes no credential at all.\n    Every OAI-PMH verb was answered with HTTP 200 on an anonymous request from a residential\n    IP with no header beyond a browser User-Agent. There is no securityScheme to declare\n    because the repository does not operate one.\nschemes: []\nsurfaces:\n  - surface: CURIS OAI-PMH harvesting endpoint\n    url: https://curis.ku.dk/ws/oai\n    x-operator: institution\n    auth: none\n    evidence: >-\n      All six OAI-PMH verbs returned 200 application/xml\
  \ unauthenticated on 2026-08-30.\n      robots.txt on the sibling portal advertises Crawl-Delay: 5; no rate-limit header was\n      returned on any probe.\n  - surface: Elsevier Pure Web Service (REST)\n    url: https://curis.ku.dk/ws/api\n    x-operator: tenant\n    auth: api-key\n    evidence: >-\n      https://curis.ku.dk/ws/api returns 200 (HTML landing page, 19,723 bytes) but\n      https://curis.ku.dk/ws/api/524/openapi.yaml returns 401. The contract exists and is\n      gated; it is also Elsevier's document, not Copenhagen's, so it is not saved in this\n      repo. Recorded as a tenant relationship in apis.yml instead.\n  - surface: University of Copenhagen SAML 2.0 identity provider\n    url: https://id.ku.dk/nidp/saml2/metadata\n    x-operator: institution\n    auth: saml2-websso\n    evidence: >-\n      Signed SAML 2.0 EntityDescriptor served at 200, 24,737 bytes, entityID\n      https://id.ku.dk/nidp/saml2/metadata. The metadata document itself is public and\n      unauthenticated\
  \ — that is what makes it a machine-readable surface — while the SSO\n      endpoints it advertises are the authentication mechanism for KUnet and ERDA.\n  - surface: Windows AD FS federation endpoint\n    url: https://federation.ku.dk/adfs/services/trust\n    x-operator: institution\n    auth: ws-federation\n    evidence: >-\n      Registered in the WAYF federation metadata but unreachable from the public internet —\n      the connection timed out after 25s on 2026-08-30. Firewalled to campus/federation\n      traffic. Recorded, not credited as a live pointer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-copenhagen/refs/heads/main/authentication/university-of-copenhagen-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Research
- Denmark
- Nordic
- Open-Source
- Research Data
- Research Repository
- Identity Federation
- OAI-PMH
- Open Data
- Research Computing
- Course Catalog
- Biodiversity
---
