---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deepcell.com
  spf: true
hosts:
- cert_expires: Aug 30 18:24:21 2026 GMT
  host: deepcell.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepcell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepCell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DeepCell
provider_slug: deepcell
slug: deepcell-domain-security
source_filename: deepcell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepcell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:24:21 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: deepcell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepcell/refs/heads/main/security/deepcell-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Life Sciences
- Single Cell Analysis
- Cell Imaging
- Morpholomics
- Deep Learning
- Biotechnology
- Drug Discovery
- Oncology
- Cell and Gene Therapy
---
