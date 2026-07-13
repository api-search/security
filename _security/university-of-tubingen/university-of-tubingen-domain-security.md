---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uni-tuebingen.de
  spf: true
hosts:
- cert_expires: Dec  1 08:00:56 2026 GMT
  host: uni-tuebingen.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 11:03:06 2026 GMT
  host: fdat.uni-tuebingen.de
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Tubingen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Tübingen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Tübingen
provider_slug: university-of-tubingen
slug: university-of-tubingen-domain-security
source_filename: university-of-tubingen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uni-tuebingen.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 08:00:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fdat.uni-tuebingen.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 11:03:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: uni-tuebingen.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-tubingen/refs/heads/main/security/university-of-tubingen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Germany
- Open Data
---
