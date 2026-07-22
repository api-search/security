---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dualbird.io
  spf: true
hosts:
- cert_expires: Oct 12 14:26:56 2026 GMT
  host: dualbird.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dualbird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dualbird, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dualbird
provider_slug: dualbird
slug: dualbird-domain-security
source_filename: dualbird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dualbird.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 14:26:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dualbird.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dualbird/refs/heads/main/security/dualbird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Data Processing
- AI Infrastructure
- Apache Spark
- Amazon EMR
- Analytics
- Hardware Acceleration
- Big Data
---
