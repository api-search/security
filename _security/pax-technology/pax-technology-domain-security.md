---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pax.us
  spf: true
hosts:
- cert_expires: Jan 10 19:33:15 2027 GMT
  host: www.pax.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pax Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PAX Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PAX Technology
provider_slug: pax-technology
slug: pax-technology-domain-security
source_filename: pax-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pax.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 19:33:15 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pax.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pax-technology/refs/heads/main/security/pax-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- POS
- FinTech
- Hardware
---
