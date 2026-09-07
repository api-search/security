---
api_specs:
- filename: elsevier-scopus-swagger.json
  format: json
  label: Elsevier Scopus APIs
  slug: elsevier-scopus-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-scopus-swagger.json
- filename: elsevier-sciencedirect-swagger.json
  format: json
  label: Elsevier ScienceDirect APIs
  slug: elsevier-sciencedirect-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-sciencedirect-swagger.json
- filename: elsevier-scival-swagger.json
  format: json
  label: Elsevier SciVal API
  slug: elsevier-scival-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-scival-swagger.json
- filename: elsevier-engineering-village-swagger.json
  format: json
  label: Elsevier Engineering Village API
  slug: elsevier-engineering-village-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-engineering-village-swagger.json
- filename: elsevier-retrieval-swagger.json
  format: json
  label: Elsevier Retrieval APIs
  slug: elsevier-retrieval-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-retrieval-swagger.json
- filename: elsevier-metadata-swagger.json
  format: json
  label: Elsevier Metadata APIs
  slug: elsevier-metadata-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-metadata-swagger.json
- filename: elsevier-abstract-api-openapi.yml
  format: yaml
  label: Elsevier Abstract API
  slug: elsevier-abstract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-abstract-api-openapi.yml
- filename: elsevier-search-api-openapi.yml
  format: yaml
  label: Elsevier Search API
  slug: elsevier-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-search-api-openapi.yml
certification_count: 1
certifications:
- ISO/IEC 27001
description: 'Elsevier publishes a corporate security and compliance page covering encryption in transit, vulnerability scanning, secure code review, bug bounties, AI data handling and privacy posture. It is a narrative page, not a document portal: no certificate, report, bridge letter or subprocessor list is downloadable from it.'
kind: trust-center
layout: security
name: Elsevier Trust Center
name_suffix: Trust Center
overview: Elsevier maintains a public trust center documenting ISO/IEC 27001 compliance.
provider_name: Elsevier
provider_slug: elsevier
slug: elsevier-trust-center
source_filename: elsevier-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://www.elsevier.com/security\nprovider: Elsevier\nproviderId: elsevier\nname: Elsevier Security & Compliance\nurl: https://www.elsevier.com/security\nhttp_status: 200\ndescription: >-\n  Elsevier publishes a corporate security and compliance page covering encryption in transit,\n  vulnerability scanning, secure code review, bug bounties, AI data handling and privacy\n  posture. It is a narrative page, not a document portal: no certificate, report, bridge letter\n  or subprocessor list is downloadable from it.\ncertifications:\n- name: ISO/IEC 27001\n  status: claimed\n  artifact_available: false\n  evidence: >-\n    \"We maintain compliance with leading security frameworks and hold certifications such as\n    ISO 27001.\" — https://www.elsevier.com/security\nprograms:\n- name: Bug bounty\n  status: claimed\n  public_program: false\n  evidence: >-\n    \"We use industry best practices such as web application firewalls,\
  \ application and\n    infrastructure vulnerability scanning, secure code reviews, bug bounties, and other\n    preventive, detective, and response controls.\"\n  note: >-\n    No program is listed on HackerOne (404) or Bugcrowd (404) under an elsevier handle, and no\n    scope, reward table or submission address is published. Probed 2026-09-06.\nprivacy:\n  regimes:\n  - GDPR\n  - CCPA\n  policy: https://www.elsevier.com/legal/privacy-policy\n  data_protection_officer: true\nai_posture:\n  evidence: >-\n    \"Our architecture and associated contracts preclude third-party model providers from\n    logging or training\" on customer inputs — https://www.elsevier.com/security\n  tdm_reservation: >-\n    Separately and machine-readably, Elsevier reserves text-and-data-mining rights over its own\n    content via /.well-known/tdmrep.json and per-response tdm-reservation headers. See\n    well-known/elsevier-well-known.yml.\ngaps:\n- name: trust portal\n  detail: https://trust.elsevier.com resolves\
  \ but returns HTTP 403 to an ordinary browser request (probed 2026-09-06).\n- name: SOC 2\n  detail: Not claimed and not published.\n- name: vulnerability disclosure policy\n  detail: >-\n    No public VDP, no security.txt on any Elsevier host, and no reporting address. Elsevier says\n    it runs bug bounties but publishes no way for a finder to reach it. See\n    security/elsevier-domain-security.yml for the transport-layer probe.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/security/elsevier-trust-center.yml
summary_line: ISO/IEC 27001
tags:
- Content
- Journals
- Medical
- Research
- Scientific
- Technical
trust_url: https://www.elsevier.com/security
---
