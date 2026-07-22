---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scalarr.io
  spf: true
hosts:
- cert_expires: Sep 10 16:04:24 2026 GMT
  host: scalarr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalarr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalarr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scalarr
provider_slug: scalarr
slug: scalarr-domain-security
source_filename: scalarr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scalarr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scalarr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalarr/refs/heads/main/security/scalarr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Fraud Detection
- Mobile Ad Fraud
- Machine Learning
- Artificial Intelligence
- Marketing
- IoT Security
---
