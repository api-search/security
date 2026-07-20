---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1010data.com
  spf: true
hosts:
- cert_expires: Sep 12 22:00:19 2026 GMT
  host: 1010data.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1010Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1010data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 1010data
provider_slug: 1010data
slug: 1010data-domain-security
source_filename: 1010data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1010data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 22:00:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 1010data.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1010data/refs/heads/main/security/1010data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Analytics
- Big Data
- Business Intelligence
- Cloud Analytics
- Data Management
- Retail Analytics
- Consumer Insights
- Capital Markets
- Data Sharing
---
