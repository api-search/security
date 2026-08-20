---
certifications: []
description: ''
kind: trust-center
layout: security
name: Chartbeat Trust Center
name_suffix: Trust Center
overview: Chartbeat maintains a public trust center covering its security and compliance posture.
provider_name: Chartbeat
provider_slug: chartbeat
slug: chartbeat-trust-center
source_filename: chartbeat-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nurl: https://trust.chartbeat.com/\nplatform: Vanta Trust Center\ncertifications: []\ncertifications_readable: false\nevidence:\n  - source: https://trust.chartbeat.com/\n    http_status: 200\n    content_type: text/html\n    signals:\n      - '<title>Chartbeat Trust Center</title>'\n      - 'canonical: https://trust.chartbeat.com'\n      - 'served by assets.vanta.com (Vanta trust-report bundle)'\n      - 'data-slugid: lb7r37f2uhw2d0yatm89q4'\n  - source: https://trust.chartbeat.com/graphql\n    http_status: 400\n    note: >-\n      The trust center renders entirely client-side from a signed GraphQL call.\n      Anonymous POSTs are rejected with \"Missing `signature` or `signedAt`\", so\n      the certification list, sub-processor list and document set are NOT\n      machine-readable without a browser session.\nnotes:\n  - >-\n    Chartbeat DOES operate a trust center at trust.chartbeat.com — the host\n    resolves, returns\
  \ 200 and is a genuine Vanta-hosted trust report page. That\n    is the verified finding recorded here.\n  - >-\n    NO named certification (SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP) could be\n    read from any public Chartbeat surface. The trust center is JS-rendered and\n    its data API requires a signed request; chartbeat.com/security/,\n    /security-policy/ and /gdpr/ all return 404. certifications is therefore an\n    honest empty list, not an assertion that Chartbeat holds none.\n  - >-\n    Because no certification could be evidenced, this file deliberately does NOT\n    carry a Compliance claim. Only GDPR and CCPA are named in Chartbeat's own\n    text, and only in the privacy policy — see conformance/.\nrelated:\n  privacy_policy: https://chartbeat.com/privacy/\n  privacy_contact: privacy@chartbeat.com\n  api_terms: https://chartbeat.com/apiterms/\n  vulnerability_disclosure: none-found\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chartbeat/refs/heads/main/security/chartbeat-trust-center.yml
summary_line: trust center published
tags:
- Company
- Software-as-a-Service
- Analytics
- Content Analytics
- Real-Time Analytics
- Audience Engagement
- Publishing
- Media
- Web Analytics
- Video Analytics
trust_url: https://trust.chartbeat.com/
---
