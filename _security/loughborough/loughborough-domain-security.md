---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lboro.ac.uk
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.lboro.ac.uk
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 21:41:22 2026 GMT
  host: koha.lboro.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: learn.lboro.ac.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loughborough Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loughborough University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Loughborough University
provider_slug: loughborough
slug: loughborough-domain-security
source_filename: loughborough-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lboro.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: koha.lboro.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 21:41:22 2026 GMT\n  hsts: false\n- host: learn.lboro.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lboro.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/security/loughborough-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Library
- Library Catalog
- Identity Federation
- Learning Management
- Research Data
- Open Access
- Repository
---
