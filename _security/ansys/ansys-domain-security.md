---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ansys.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pyansys.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.ansys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 09:21:46 2026 GMT
  host: docs.pyansys.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ansys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansys, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ansys
provider_slug: ansys
slug: ansys-domain-security
source_filename: ansys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ansys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\n- host: docs.pyansys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:21:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: ansys.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pyansys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansys/refs/heads/main/security/ansys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Simulation
- Engineering
- CAE
- CFD
- FEA
- Electromagnetics
- Multiphysics
- Cloud
- Python
- SDK
---
