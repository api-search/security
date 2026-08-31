---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: speedata.io
  spf: true
hosts:
- cert_expires: Oct 19 05:38:46 2026 GMT
  host: www.speedata.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speedata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speedata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Speedata
provider_slug: speedata
slug: speedata-domain-security
source_filename: speedata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.speedata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 05:38:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: speedata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speedata/refs/heads/main/security/speedata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Hardware Acceleration
- Analytics
- Big Data
- Apache Spark
- Data Engineering
- Artificial Intelligence
- Data Infrastructure
- Israel
---
