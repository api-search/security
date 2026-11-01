---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verusen.com
  spf: true
hosts:
- cert_expires: Jan 10 20:37:05 2027 GMT
  host: verusen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Verusen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verusen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verusen
provider_slug: verusen
slug: verusen-domain-security
source_filename: verusen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verusen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 20:37:05 2027 GMT\n  hsts: false\ndomains:\n- domain: verusen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/verusen/security/verusen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- MRO
- Inventory
- Optimization
- Manufacturing
---
