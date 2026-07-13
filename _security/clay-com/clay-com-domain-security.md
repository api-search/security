---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clay.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.clay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 21:12:16 2026 GMT
  host: university.clay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: app.clay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clay Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clay
provider_slug: clay-com
slug: clay-com-domain-security
source_filename: clay-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: university.clay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 21:12:16 2026 GMT\n  hsts: false\n- host: app.clay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/security/clay-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Prospecting
- GTM
- Sales
- Enrichment
- Automation
- AI
- Webhooks
---
