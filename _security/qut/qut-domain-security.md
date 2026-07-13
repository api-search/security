---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qut.edu.au
  spf: true
hosts:
- cert_expires: Sep 27 05:48:53 2026 GMT
  host: www.qut.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: www.library.qut.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 23:59:59 2026 GMT
  host: eprints.qut.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Queensland University of Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Queensland University of Technology
provider_slug: qut
slug: qut-domain-security
source_filename: qut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qut.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:48:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.library.qut.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eprints.qut.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qut.edu.au\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qut/refs/heads/main/security/qut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Australia
- OAI-PMH
---
