---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: southampton.ac.uk
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.southampton.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 04:23:48 2026 GMT
  host: data.southampton.ac.uk
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 06:09:18 2026 GMT
  host: sparql.data.southampton.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Southampton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Southampton, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Southampton
provider_slug: university-of-southampton
slug: university-of-southampton-domain-security
source_filename: university-of-southampton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.southampton.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.southampton.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: sparql.data.southampton.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:09:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: southampton.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/security/university-of-southampton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Linked Data
- SPARQL
- OAI-PMH
- Research
- United Kingdom
---
