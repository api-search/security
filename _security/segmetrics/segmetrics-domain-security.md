---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: segmetrics.io
  spf: true
hosts:
- cert_expires: Sep 24 02:00:11 2026 GMT
  host: segmetrics.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 15:03:19 2026 GMT
  host: developers.segmetrics.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 20:04:04 2026 GMT
  host: import.segmetrics.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Segmetrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SegMetrics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SegMetrics
provider_slug: segmetrics
slug: segmetrics-domain-security
source_filename: segmetrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: segmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:00:11 2026 GMT\n  hsts: false\n- host: developers.segmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:03:19 2026 GMT\n  hsts: false\n- host: import.segmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:04:04 2026 GMT\n  hsts: false\ndomains:\n- domain: segmetrics.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segmetrics/refs/heads/main/security/segmetrics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- Analytics
- Attribution
- Marketing Analytics
- Reporting
- Business Intelligence
- Advertising
- SaaS
- MCP
---
