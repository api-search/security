---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 1lookup.io
  spf: true
hosts:
- cert_expires: Sep 28 22:00:53 2026 GMT
  host: app.1lookup.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:05:21 2026 GMT
  host: www.1lookup.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Lookup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1Lookup, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 1Lookup
provider_slug: 1lookup
slug: 1lookup-domain-security
source_filename: 1lookup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.1lookup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:00:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.1lookup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:05:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 1lookup.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1lookup/refs/heads/main/security/1lookup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- phone validation
- email validation
- IP intelligence
- fraud & risk
- data enrichment
- B2B contact & company data
- SEO / web analytics
- audio transcription
- MCP / agent-native
- REST API
---
