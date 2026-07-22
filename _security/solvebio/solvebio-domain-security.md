---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: solvebio.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.solvebio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.solvebio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solvebio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SolveBio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SolveBio
provider_slug: solvebio
slug: solvebio-domain-security
source_filename: solvebio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solvebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\n- host: api.solvebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: solvebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solvebio/refs/heads/main/security/solvebio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Genomics
- Bioinformatics
- Life Sciences
- Precision Medicine
- Biomedical Data
- Datasets
- SDK
---
