---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: upf.edu
  spf: true
hosts:
- cert_expires: Aug 22 07:11:47 2026 GMT
  host: www.upf.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: data.upf.edu
  https: false
- cert_expires: Nov 26 12:46:18 2026 GMT
  host: repositori.upf.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Universitat Pompeu Fabra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universitat Pompeu Fabra, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Universitat Pompeu Fabra
provider_slug: universitat-pompeu-fabra
slug: universitat-pompeu-fabra-domain-security
source_filename: universitat-pompeu-fabra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upf.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:11:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.upf.edu\n  https: false\n- host: repositori.upf.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 12:46:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upf.edu\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universitat-pompeu-fabra/refs/heads/main/security/universitat-pompeu-fabra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Research
- Library
- Repository
- SPARQL
- OAI-PMH
- Spain
- Barcelona
---
