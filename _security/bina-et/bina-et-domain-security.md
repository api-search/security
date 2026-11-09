---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bina.et
  spf: true
hosts:
- cert_expires: Jan 11 10:36:38 2027 GMT
  host: bina.et
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bina Et Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BinaSmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BinaSmart
provider_slug: bina-et
slug: bina-et-domain-security
source_filename: bina-et-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bina.et\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 10:36:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bina.et\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bina-et/security/bina-et-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Super App
- Ethiopia
- Ride Hailing
- Payments
- Entertainment
---
