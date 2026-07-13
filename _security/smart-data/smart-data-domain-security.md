---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: smart-data.com
  spf: false
hosts:
- cert_expires: Aug 19 00:52:11 2026 GMT
  host: www.smart-data.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smart Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smart Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Smart Data
provider_slug: smart-data
slug: smart-data-domain-security
source_filename: smart-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smart-data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 00:52:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: smart-data.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smart-data/refs/heads/main/security/smart-data-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Analytics
- Data Integration
- Data Management
- Data Enrichment
- Data Quality
- Real-Time Processing
- Master Data Management
- Streaming
---
