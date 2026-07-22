---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dimensional.me
  spf: false
hosts:
- cert_expires: Aug 24 13:02:35 2026 GMT
  host: www.dimensional.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dimensional Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dimensional, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dimensional
provider_slug: dimensional
slug: dimensional-domain-security
source_filename: dimensional-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dimensional.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:02:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dimensional.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dimensional/refs/heads/main/security/dimensional-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Personality Science
- Psychology
- Consumer
- Mobile Application
- Social
- Relationships
- Assessment
---
