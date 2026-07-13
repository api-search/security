---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: curtin.edu.au
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: researchdata.edu.au
  spf: false
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.curtin.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: espace.curtin.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  1 08:40:30 2026 GMT
  host: researchdata.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curtin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curtin University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Curtin University
provider_slug: curtin
slug: curtin-domain-security
source_filename: curtin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curtin.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n- host: espace.curtin.edu.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\n- host: researchdata.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:40:30 2026 GMT\n  hsts: false\ndomains:\n- domain: curtin.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: researchdata.edu.au\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curtin/refs/heads/main/security/curtin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- Australia
---
