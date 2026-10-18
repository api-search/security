---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: treyd.io
  spf: true
hosts:
- cert_expires: Jan 10 01:03:04 2027 GMT
  host: treyd.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Treyd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treyd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Treyd
provider_slug: treyd
slug: treyd-domain-security
source_filename: treyd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: treyd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:03:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: treyd.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treyd/refs/heads/main/security/treyd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- WorkingCapital
- B2B
- Europe
---
