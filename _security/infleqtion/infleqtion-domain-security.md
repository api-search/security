---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infleqtion.com
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Oct  3 10:46:00 2026 GMT
  host: www.infleqtion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: superstaq.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infleqtion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infleqtion, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Infleqtion
provider_slug: infleqtion
slug: infleqtion-domain-security
source_filename: infleqtion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infleqtion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:46:00 2026 GMT\n  hsts: false\n- host: superstaq.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infleqtion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infleqtion/refs/heads/main/security/infleqtion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum Computing
- Quantum Software
- Neutral Atom
- Atomic Clocks
- Quantum Sensing
- Superstaq
- Sqale
- Tiqker
- Rydberg
- Inertial Sensing
- Hardware
- Research
---
