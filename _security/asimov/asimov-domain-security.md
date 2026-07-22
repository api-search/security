---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: asimov.io
  spf: true
hosts:
- cert_expires: Aug 28 19:55:25 2026 GMT
  host: www.asimov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asimov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asimov, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Asimov
provider_slug: asimov
slug: asimov-domain-security
source_filename: asimov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asimov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:55:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asimov.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asimov/refs/heads/main/security/asimov-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Synthetic Biology
- Biotechnology
- Genetic Design
- Cell Line Development
- Gene Therapy
- Bioinformatics
- Life Sciences
---
