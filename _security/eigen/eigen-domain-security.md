---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eigentech.com
  spf: true
hosts:
- cert_expires: Oct 12 18:30:24 2026 GMT
  host: eigentech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eigen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eigen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eigen
provider_slug: eigen
slug: eigen-domain-security
source_filename: eigen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eigentech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:30:24 2026 GMT\n  hsts: null\ndomains:\n- domain: eigentech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eigen/refs/heads/main/security/eigen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Document AI
- Intelligent Document Processing
- Data Extraction
- Natural Language Processing
- Machine Learning
- Financial Services
- Legal Tech
- Insurance
---
