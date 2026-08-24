---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inbrace.com
  spf: true
hosts:
- cert_expires: Nov 16 17:33:38 2026 GMT
  host: inbrace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: inbrace.com resolves to Cloudflare and answers HTTP 301 on every path probed (apex, /.well-known/*, /openapi.json, /llms.txt, /docs, /api), redirecting wholesale to https://insmilebraces.com/ — the site of InSmile Braces, the separate company that acquired the InBrace IP after Swift Health Systems, Inc. ceased operations in April 2025. The TLS/HSTS/DNS posture recorded here therefore describes the domain as it is operated today by the successor, not any surviving InBrace origin.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inbrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InBrace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InBrace
provider_slug: inbrace
slug: inbrace-domain-security
source_filename: inbrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inbrace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 17:33:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    inbrace.com resolves to Cloudflare and answers HTTP 301 on every path probed\n    (apex, /.well-known/*, /openapi.json, /llms.txt, /docs, /api), redirecting wholesale\n    to https://insmilebraces.com/ — the site of InSmile Braces, the separate company that\n    acquired the InBrace IP after Swift Health Systems, Inc. ceased operations in April\n    2025. The TLS/HSTS/DNS posture recorded here therefore describes the domain as it is\n    operated today by the successor, not any surviving InBrace origin.\ndomains:\n- domain: inbrace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inbrace/refs/heads/main/security/inbrace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Orthodontics
- Dental
- Medical Devices
- Health
- Lingual Braces
- Consumer Health
- Defunct
---
