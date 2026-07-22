---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: provenmetal.com
  spf: true
hosts:
- cert_expires: Sep  2 21:21:26 2026 GMT
  host: provenmetal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 21:21:26 2026 GMT
  host: order.provenmetal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Provenmetal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Provenmetal, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Provenmetal
provider_slug: provenmetal
slug: provenmetal-domain-security
source_filename: provenmetal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: provenmetal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:21:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: order.provenmetal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:21:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: provenmetal.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provenmetal/refs/heads/main/security/provenmetal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PCB
- Printed Circuit Boards
- Electronics Manufacturing
- Hardware
- Contract Manufacturing
- Reshoring
- Y Combinator
---
