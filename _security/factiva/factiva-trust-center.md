---
api_specs:
- filename: factiva-apis
  format: yaml
  label: Factiva Snapshots API
  slug: factiva-snapshots-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Streams API
  slug: factiva-streams-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Extractions API
  slug: factiva-extractions-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Analytics API
  slug: factiva-analytics-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva DJID Taxonomy API
  slug: factiva-djid-taxonomy-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Code API
  slug: factiva-code-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-content-api-openapi.yml
  format: yaml
  label: Factiva Content API
  slug: factiva-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-content-api-openapi.yml
- filename: factiva-content-search-api-openapi.yml
  format: yaml
  label: Factiva Content Search API
  slug: factiva-content-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-content-search-api-openapi.yml
- filename: factiva-default-api-openapi.yml
  format: yaml
  label: Factiva Default API
  slug: factiva-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-default-api-openapi.yml
- filename: factiva-editions-api-openapi.yml
  format: yaml
  label: Factiva Editions API
  slug: factiva-editions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-editions-api-openapi.yml
- filename: factiva-newsletters-api-openapi.yml
  format: yaml
  label: Factiva Newsletters API
  slug: factiva-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-newsletters-api-openapi.yml
certifications:
- ISO/IEC 27001
- ISAE 3000
description: Dow Jones publishes no dedicated trust center (trust.dowjones.com and security.dowjones.com do not resolve). It does publish a named certification page whose scope explicitly includes Factiva, plus a vulnerability disclosure policy and an assurance-report page, which together are the compliance posture a Factiva buyer can actually read without a sales conversation.
kind: trust-center
layout: security
name: Factiva Trust Center
name_suffix: Trust Center
overview: Factiva maintains a public trust center documenting ISO/IEC 27001 and ISAE 3000 compliance.
provider_name: Factiva
provider_slug: factiva
slug: factiva-trust-center
source_filename: factiva-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://www.dowjones.com/iso-certification/\ndescription: >-\n  Dow Jones publishes no dedicated trust center (trust.dowjones.com and security.dowjones.com\n  do not resolve). It does publish a named certification page whose scope explicitly includes\n  Factiva, plus a vulnerability disclosure policy and an assurance-report page, which together\n  are the compliance posture a Factiva buyer can actually read without a sales conversation.\ntrust_center: false\ntrust_center_note: >-\n  No consolidated trust portal. Certification and security policy are published as individual\n  pages on www.dowjones.com and linked from the site footer.\npages:\n  - url: https://www.dowjones.com/iso-certification/\n    title: ISO 27001 Certification\n    http_status: 200\n  - url: https://www.dowjones.com/security/\n    title: Dow Jones Vulnerability Disclosure Program\n    http_status: 200\n  - url: https://www.dowjones.com/privacy-notice/\n\
  \    title: Privacy Notice\n    http_status: 200\ncertifications:\n  - name: ISO/IEC 27001\n    scope: >-\n      Dow Jones Inc.'s Information Security Management System (ISMS) is certified as conforming\n      to ISO 27001. The published certification scope covers the information security framework\n      and associated activities relating to Risk & Compliance and to Factiva Newsplus.\n    covers_factiva: true\n    audit_cycle: >-\n      Three-year certification cycle with renewal audits, plus annual surveillance (touch point)\n      audits.\n    auditor: Schellman\n    certificate_published: true\n    source: https://www.dowjones.com/iso-certification/\n  - name: ISAE 3000\n    scope: >-\n      Dow Jones publishes ISAE 3000 and data quality reports; the footer link is scoped to the\n      Risk & Compliance product line rather than to Factiva.\n    covers_factiva: unknown\n    source: https://www.dowjones.com/\n    note: >-\n      Recorded as published-but-not-Factiva-scoped. Do not claim\
  \ ISAE 3000 coverage for the\n      Factiva APIs without a scope statement from Dow Jones.\nnot_found:\n  - https://trust.dowjones.com\n  - https://security.dowjones.com\n  - https://www.dowjones.com/compliance/\nevidence:\n  - source: https://www.dowjones.com/iso-certification/\n    http_status: 200\n    fetched: '2026-08-13'\n    keywords:\n      - iso 27001\n      - information security management system\n      - factiva newsplus\n      - surveillance audits\n      - schellman\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/security/factiva-trust-center.yml
summary_line: ISO/IEC 27001, ISAE 3000
tags:
- Artificial Intelligence
- Business Intelligence
- Content Aggregation
- Enterprise Data
- GenAI
- Market Data
- Media Monitoring
- News
- News API
- Research
- Taxonomy
trust_url: ''
---
