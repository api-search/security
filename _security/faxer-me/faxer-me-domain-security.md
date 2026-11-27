---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: faxer.me
  spf: true
hosts:
- cert_expires: Jan  3 05:22:09 2027 GMT
  host: faxer.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Faxer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faxer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Faxer
provider_slug: faxer-me
slug: faxer-me-domain-security
source_filename: faxer-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faxer.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 05:22:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: faxer.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/faxer-me/security/faxer-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fax
- Online Fax
- Software-as-a-Service
- Payments
- Communications
---
