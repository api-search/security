---
api_specs:
- filename: searchapi-search-api-openapi.yml
  format: yaml
  label: SearchApi SERP API
  slug: searchapi-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/openapi/searchapi-search-api-openapi.yml
- filename: searchapi-account-api-openapi.yml
  format: yaml
  label: SearchApi Account & Analytics API
  slug: searchapi-account-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/openapi/searchapi-account-api-openapi.yml
- filename: searchapi-analytics-api-openapi.yml
  format: yaml
  label: SearchApi Analytics API
  slug: searchapi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/openapi/searchapi-analytics-api-openapi.yml
certifications:
- ISO/IEC 27001:2022
- GDPR
- SOC 2
- PCI DSS
- HIPAA
- FedRAMP
description: ''
kind: trust-center
layout: security
name: Searchapi Trust Center
name_suffix: Trust Center
overview: SearchApi maintains a public trust center documenting ISO/IEC 27001:2022, GDPR, SOC 2, PCI DSS, HIPAA, and FedRAMP compliance.
provider_name: SearchApi
provider_slug: searchapi
slug: searchapi-trust-center
source_filename: searchapi-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.searchapi.io/announcements\ntrust_center:\n  url: https://security.searchapi.io/\n  status: 200\n  title: Trust center\n  discovered_via: >-\n    Linked from the site footer and named in the July 2026 changelog entry\n    (published 2026-08-06): \"GDPR documentation sits alongside our ISO/IEC 27001:2022\n    certificate in our Trust Center.\"\n  machine_readable: false\n  note: >-\n    The trust center is a Vite single-page application. The HTML served to a non-JS client\n    is a 604-byte shell containing only `<title>Trust center</title>`; the certificate and\n    policy inventory is rendered client-side, and the SPA's catch-all answers HTTP 200\n    with that same shell for every path probed (including /.well-known/security.txt and\n    /.well-known/agent-card.json). The JS bundle exposes no fetchable JSON API. So the\n    trust center is REAL and it is the provider's own host, but its contents are not\n    machine-readable\
  \ and the certifications below are sourced from SearchApi's own dated\n    announcements rather than from the trust center document itself.\ncertifications:\n  - name: ISO/IEC 27001:2022\n    status: certified\n    announced: '2026-07-02'\n    source: https://www.searchapi.io/announcements\n    evidence: >-\n      \"ISO/IEC 27001:2022 Certified — The certification covers our information security\n      management system, including how we manage infrastructure...\" (June 2026 update,\n      published 2026-07-02). Certificate is stated to be available in the Trust Center.\n  - name: GDPR\n    status: compliant\n    announced: '2026-08-06'\n    source: https://www.searchapi.io/announcements\n    evidence: >-\n      \"GDPR Compliant — Our data protection program covers how we collect, process, store,\n      and delete personal data, along with subprocessors...\" (July 2026 update, published\n      2026-08-06). Documentation stated to sit in the Trust Center alongside the ISO\n      certificate.\n\
  \    dpa: https://www.searchapi.io/legal/dpa\n  - name: SOC 2\n    status: not-published\n    note: No SOC 2 report or Type I/II claim is published anywhere on the provider's surface.\n  - name: PCI DSS\n    status: not-applicable\n    note: SearchApi does not process cardholder data on behalf of customers.\n  - name: HIPAA\n    status: not-published\n  - name: FedRAMP\n    status: not-published\ndata_handling:\n  zero_retention:\n    available: true\n    tier: enterprise\n    mechanism: '`zero_retention=true` request parameter on search, account and analytics endpoints'\n    description: Disables logging and storage of the request for compliance purposes.\n    source: https://www.searchapi.io/docs/account-api\n  dpa: https://www.searchapi.io/legal/dpa\n  privacy_policy: https://www.searchapi.io/legal/privacy\n  subprocessors:\n    published_url: null\n    note: >-\n      Subprocessor coverage is asserted in the GDPR announcement but no public\n      subprocessor list URL was found outside\
  \ the JS-rendered trust center.\ngaps:\n  - No security.txt on any host (probed www.searchapi.io, searchapi.io, security.searchapi.io -> 404 / SPA shell).\n  - No published vulnerability disclosure policy or bug-bounty program (HackerOne/Bugcrowd/Intigriti all miss).\n  - Trust center contents are JS-rendered and not machine-readable.\nrefs:\n  conformance: conformance/searchapi-conformance.yml\n  vulnerability_disclosure: null\n  domain_security: security/searchapi-domain-security.yml\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/security/searchapi-trust-center.yml
summary_line: ISO/IEC 27001:2022, GDPR, SOC 2, PCI DSS, HIPAA, FedRAMP
tags:
- Search
- serp-api
- google-search
- Web Scraping
- search-data
- Market Intelligence
- SEO
- MCP
- agent-native
trust_url: ''
---
