---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: di.gg
  spf: false
hosts:
- cert_expires: Aug 22 04:47:50 2026 GMT
  host: di.gg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Digg
provider_slug: digg
slug: digg-domain-security
source_filename: digg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: di.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 04:47:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: di.gg\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digg/refs/heads/main/security/digg-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- News Aggregation
- Social News
- Content Curation
- Technology
- Media
- Artificial Intelligence
---
