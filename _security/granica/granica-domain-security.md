---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: granica.ai
  spf: true
hosts:
- cert_expires: Oct 13 01:54:33 2026 GMT
  host: www.granica.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 01:13:45 2026 GMT
  host: docs.granica.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Granica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Granica, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Granica
provider_slug: granica
slug: granica-domain-security
source_filename: granica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.granica.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 01:54:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.granica.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 01:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: granica.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granica/refs/heads/main/security/granica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Storage
- Analytics
- Artificial Intelligence
- Machine Learning
- Data Lakehouse
- Cloud Cost Optimization
- Compression
- Data Infrastructure
---
