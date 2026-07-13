---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pasqal.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Aug 25 00:34:26 2026 GMT
  host: www.pasqal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 04:11:27 2026 GMT
  host: docs.pasqal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: pulser.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pasqal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pasqal, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pasqal
provider_slug: pasqal
slug: pasqal-domain-security
source_filename: pasqal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pasqal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:34:26 2026 GMT\n  hsts: false\n- host: docs.pasqal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 04:11:27 2026 GMT\n  hsts: false\n- host: pulser.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pasqal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pasqal/refs/heads/main/security/pasqal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Quantum Computing
- Neutral Atom
- Quantum
- QPU
- Rydberg
- Pulse-Level Control
- Analog Quantum
- Digital Quantum
- HPC
- Optimization
- Quantum Machine Learning
- Quantum Simulation
- France
---
