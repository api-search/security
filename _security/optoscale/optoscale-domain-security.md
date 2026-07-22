---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: optoscale.no
  spf: true
hosts:
- cert_expires: Sep 28 10:49:18 2026 GMT
  host: optoscale.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optoscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optoscale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Optoscale
provider_slug: optoscale
slug: optoscale-domain-security
source_filename: optoscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optoscale.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:49:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: optoscale.no\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optoscale/refs/heads/main/security/optoscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Aquaculture
- Fish Farming
- Monitoring
- Computer Vision
- Edge Computing
- Artificial Intelligence
- IoT
- Data Integration
- Salmon
---
