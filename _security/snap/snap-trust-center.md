---
api_specs:
- filename: snap-conversions-api-v3-openapi.yml
  format: yaml
  label: Snap Conversions API
  slug: snap-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/openapi/snap-conversions-api-v3-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Snap Trust Center
name_suffix: Trust Center
overview: Snap maintains a public trust center covering its security and compliance posture.
provider_name: Snap
provider_slug: snap
slug: snap-trust-center
source_filename: snap-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nsource: https://trust.snap.com/\nurl: https://trust.snap.com/\napi: Snap\nsummary: >-\n  Snap Inc. publishes a trust center at trust.snap.com — a hosted \"Snap\n  Assurance Profile\" running on SecurityPal. The profile is live and published\n  (publishedAt 2026-07-28), belongs to Snap Inc., and advertises that document\n  downloads are allowed. The certification list itself is loaded client-side and\n  was not readable anonymously.\n\nvendor: SecurityPal\nprofile:\n  company_name: Snap Inc.\n  title: \"Snap Inc.'s Trust Center\"\n  html_title: Snap Assurance Profile\n  published_at: '2026-07-28'\n  document_downloads_allowed: true\n  access: >-\n    Document access is gated behind the profile's own request flow; the served\n    HTML embeds only the profile header, not its sections.\n\ncertifications: []\ncertifications_note: >-\n  NO certifications are recorded because none could be read. The page returns\n  HTTP 200 with\
  \ a React shell whose embedded JSON payload carries the profile\n  header only — no SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP, GDPR or CSA STAR\n  string appears anywhere in the served bytes, and the SecurityPal section API\n  was not reachable anonymously. Recording an empty list is the honest result:\n  Snap may well hold these reports, but a machine reading trust.snap.com cannot\n  confirm it, and this pipeline does not assert a certification it did not see.\n\nrelated:\n  - name: Snap Transparency Report\n    url: https://values.snap.com/privacy/transparency\n    status: 200\n    note: Semi-annual transparency reporting; not a security certification surface.\n  - name: Snap Privacy Center\n    url: https://values.snap.com/privacy/privacy-policy\n  - name: Snap Developer Terms\n    url: https://www.snap.com/terms/developer\n  - name: Vulnerability disclosure / bug bounty\n    url: https://hackerone.com/snapchat\n    ref: security/snap-vulnerability-disclosure.yml\n\nx-evidence:\n  -\
  \ fetched: '2026-08-13'\n    url: https://trust.snap.com/\n    http_status: 200\n    content_type: text/html\n    finding: >-\n      Embedded application/json payload identifies companyName \"Snap Inc.\",\n      profileName \"snap\", htmlHeadTitle \"Snap Assurance Profile\",\n      documentDownloadsAllowed true, publishedAt 2026-07-28.\n  - fetched: '2026-08-13'\n    url: https://values.snap.com/privacy/transparency\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/security/snap-trust-center.yml
summary_line: trust center published
tags:
- Company
- Advertising
- Marketing
- Social-Media
- Augmented Reality
- Camera
- Authentication
- Identity
- Conversions
- Attribution
- SDK
trust_url: https://trust.snap.com/
---
