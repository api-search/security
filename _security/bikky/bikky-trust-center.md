---
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Bikky Trust Center
name_suffix: Trust Center
overview: Bikky maintains a public trust center documenting SOC 2 compliance.
provider_name: Bikky
provider_slug: bikky
slug: bikky-trust-center
source_filename: bikky-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.bikky.com/\nplatform: Vanta\ncertifications:\n  - SOC 2\nframeworks_referenced:\n  - NIST (system design and security policies stated as aligned with NIST best practices)\npractices_published:\n  - Customer data encrypted at rest\n  - Regular vulnerability scanning\n  - Regular penetration tests\n  - Regular policy reviews\n  - Customers own their data; stated compliance with US data privacy regulations\nevidence:\n  - source: https://trust.bikky.com/\n    http_status: 200\n    kind: trust-center\n    detail: >-\n      Serves <title>Bikky Trust Center</title> and og:title \"Bikky Trust Center\"\n      from the Vanta trust-report bundle (assets.vanta.com index-trust-report).\n      DNS confirms provider ownership: trust.bikky.com is a CNAME to\n      662bd7f45360cc947af486cc.cname.vantatrust.com.\n  - source: https://www.bikky.com/\n    http_status: 200\n    kind: security-section\n    detail: >-\n  \
  \    Homepage \"Security & privacy\" section states \"SOC 2 Certified — We're proud\n      to be SOC 2 certified, the leading industry standard for enterprise-level\n      protection\", \"All customer data is fully encrypted at rest and we undergo\n      regular vulnerability scanning, penetration tests, and policy reviews\", and\n      links to the trust center at https://trust.bikky.com/.\nmachine_readability:\n  readable: false\n  note: >-\n    The Vanta trust report renders client-side. Its GraphQL backend at\n    /graphql rejects anonymous queries with \"Missing `signature` or `signedAt`\"\n    (HTTP 400), so the certification list, audit reports and subprocessors are\n    not retrievable without a signed session. The SOC 2 certification recorded\n    above is taken from the provider's own homepage copy, not from the trust\n    center DOM.\nvulnerability_disclosure:\n  published: false\n  note: >-\n    Bikky publishes security PRACTICES (scanning, pen tests) but no channel for\n \
  \   third parties to REPORT a vulnerability — no security.txt on any host, no\n    /security or /responsible-disclosure page, no bug bounty program on\n    HackerOne/Bugcrowd/Intigriti, and no security@ address in the privacy policy\n    or terms (the only published address is support@bikky.com). No\n    VulnerabilityDisclosure or Security pointer is wired as a result.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bikky/refs/heads/main/security/bikky-trust-center.yml
summary_line: SOC 2
tags:
- Restaurant
- Customer Data Platform
- Guest Analytics
- Integrations
- Marketing
- Loyalty
trust_url: https://trust.bikky.com/
---
