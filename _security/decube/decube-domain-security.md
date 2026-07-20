---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: decube.io
  spf: true
hosts:
- cert_expires: Oct 15 12:02:22 2026 GMT
  host: decube.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 02:30:19 2026 GMT
  host: docs.decube.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: connect.us1.decube.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Decube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decube, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Decube
provider_slug: decube
slug: decube-domain-security
source_filename: decube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decube.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:02:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.decube.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:30:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.us1.decube.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: decube.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decube/refs/heads/main/security/decube-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Observability
- Data Governance
- Data Catalog
- Data Quality
- Data Lineage
- Metadata Management
- Data Trust
- Data Products
- Model Context Protocol
---
