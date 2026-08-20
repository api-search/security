---
api_specs:
- filename: ahrefs-openapi-original.json
  format: json
  label: Ahrefs API v3
  slug: api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahrefs/refs/heads/main/openapi/_original/ahrefs-openapi-original.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Ahrefs Trust Center
name_suffix: Trust Center
overview: Ahrefs maintains a public trust center covering its security and compliance posture.
provider_name: Ahrefs
provider_slug: ahrefs
slug: ahrefs-trust-center
source_filename: ahrefs-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nprobe: true\nurl: https://trust.ahrefs.com/\ncanonical: https://trust.ahrefs.com/en\nevidence:\n- source: https://trust.ahrefs.com/\n  http_status: 200\n  content_type: text/html; charset=utf-8\n  title: Compliance at Ahrefs.\n  og_title: Compliance at Ahrefs.\n  fetched: '2026-08-12'\n- source: https://trust.ahrefs.com/ Content-Security-Policy header\n  observation: 'connect-src and img-src allow https://eu.probo.com and a Probo S3 bucket'\n  inference: the trust center is hosted on Probo (getprobo.com)\ncertifications: []\ncertifications_note: >-\n  NONE ENUMERATED — not \"none held\". The trust center is a client-rendered single-page app: the served\n  HTML contains only the document head and a skeleton, and every content path (including the GraphQL\n  endpoints tried) returns the same SPA shell with content-type text/html. No certification names could\n  be read from the page anonymously, so none are recorded here. Third-party sources\
  \ report SOC 2 Type 2\n  and ISO 27001 for Ahrefs Pte. Ltd., but they are not the provider's own published surface and are\n  deliberately not asserted as evidence in this artifact.\nlocalized: true\nlocales:\n- en\n- de\n- es\n- fr\n- id\n- it\n- ja\n- ko\n- nl\n- pl\n- pt\n- tr\n- uk\n- zh\ndocument_access: >-\n  Probo trust centers gate audit reports behind an access request; no document could be listed or\n  downloaded anonymously.\nrelated:\n  privacy_policy: https://ahrefs.com/privacy-policy\n  terms: https://ahrefs.com/terms\n  legal_entity: Ahrefs Pte. Ltd. (201227417H), 16 Raffles Quay #33-03, Hong Leong Building, Singapore\nsecurity_txt:\n  present: false\n  probed:\n  - url: https://ahrefs.com/.well-known/security.txt\n    status: 404\n  - url: https://api.ahrefs.com/.well-known/security.txt\n    status: 404\n  - url: https://docs.ahrefs.com/.well-known/security.txt\n    status: 404\n  - url: https://app.ahrefs.com/.well-known/security.txt\n    status: 404\nvulnerability_disclosure:\n\
  \  present: false\n  note: >-\n    No security.txt, no /security or /responsible-disclosure page (https://ahrefs.com/security 404s),\n    and no HackerOne/Bugcrowd/Intigriti program found. probe-security-programs.py returned\n    vdp=none. No VulnerabilityDisclosure or Security pointer is emitted — a security-disclosure\n    channel could not be verified.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahrefs/refs/heads/main/security/ahrefs-trust-center.yml
summary_line: trust center published
tags:
- Company
- SEO
- Marketing
- Search
- Analytics
- Backlinks
- Keywords
- Web Analytics
- Rank Tracking
- Site Audit
- Brand Monitoring
- Social-Media
trust_url: https://trust.ahrefs.com/
---
