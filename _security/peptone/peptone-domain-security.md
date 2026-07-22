---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: peptone.io
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: peptone.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peptone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peptone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Peptone
provider_slug: peptone
slug: peptone-domain-security
source_filename: peptone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peptone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: peptone.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peptone/refs/heads/main/security/peptone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotech
- Drug Discovery
- Proteins
- Machine Learning
- Protein Engineering
- Intrinsically Disordered Proteins
---
