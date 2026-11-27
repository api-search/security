---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dimensionkit.com
  spf: true
hosts:
- cert_expires: Jan 30 15:30:47 2027 GMT
  host: dimensionkit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DimensionKit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DimensionKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DimensionKit
provider_slug: dimensionkit-com
slug: dimensionkit-com-domain-security
source_filename: dimensionkit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dimensionkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 15:30:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dimensionkit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dimensionkit-com/security/dimensionkit-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Assessment
- Scorecards
- Lead Generation
- MCP
- Artificial Intelligence
- Quizzes
---
