---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alluxio.io
  spf: false
hosts:
- cert_expires: Aug 20 15:13:22 2026 GMT
  host: www.alluxio.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 22:46:43 2026 GMT
  host: documentation.alluxio.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alluxio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alluxio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Alluxio
provider_slug: alluxio
slug: alluxio-domain-security
source_filename: alluxio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alluxio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:13:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.alluxio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:46:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alluxio.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alluxio/refs/heads/main/security/alluxio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Data Orchestration
- Data Caching
- AI Infrastructure
- Machine Learning
- Analytics
- Distributed Storage
- Object Storage
- S3
- Open Source
---
