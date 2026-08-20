---
certifications: []
description: ''
kind: trust-center
layout: security
name: Paramark Trust Center
name_suffix: Trust Center
overview: Paramark maintains a public trust center covering its security and compliance posture.
provider_name: Paramark
provider_slug: paramark
slug: paramark-trust-center
source_filename: paramark-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://trust.paramark.com/\ntrust_center:\n  url: https://trust.paramark.com/\n  http_status: 200\n  title: Paramark.com Trust Center\n  platform: Vanta (assets served from assets.vanta.com; the page is Vanta's\n    index-trust-report bundle)\n  fronted_by: Cloudflare\ncertifications_published: unknown\ncertifications: []\ndocuments:\n  request_flow: https://app.vanta.com/doc\n  note: The page links document requests through app.vanta.com/doc, which requires\n    a request/NDA flow.\nnote: >-\n  Paramark runs a real trust center on its own subdomain and it answers HTTP 200. It is a Vanta\n  trust report rendered entirely client-side: the served HTML is a 7,069-byte shell containing\n  only the page title and Vanta's script bundle, and the report content is fetched by an Apollo\n  GraphQL client after script execution. No certification name — SOC 2, ISO 27001, GDPR, CCPA,\n  HIPAA, PCI DSS — appears anywhere in the served markup,\
  \ so none is recorded here and no\n  Compliance pointer is emitted. Presence is verified; content is not readable by a machine.\n  This is a js-rendered-docs failure on an otherwise good provider practice.\nrelated:\n  vulnerability_disclosure: none found — /.well-known/security.txt returns 404 on\n    paramark.com, api.paramark.com and signin.paramark.com; no bug bounty program\n    (HackerOne, Bugcrowd, Intigriti) and no disclosure page were found.\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://trust.paramark.com/\n  http_status: 200\n  content_type: text/html\n  bytes: 7069\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paramark/refs/heads/main/security/paramark-trust-center.yml
summary_line: trust center published
tags:
- Company
- Application
- Marketing
- Analytics
- Measurements
- Marketing Mix Modeling
- Incrementality
- Advertising
- Artificial Intelligence
trust_url: ''
---
