---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airops.com
  spf: true
hosts:
- cert_expires: Sep 11 06:57:08 2026 GMT
  host: www.airops.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 09:11:30 2026 GMT
  host: docs.airops.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.airops.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirOps, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AirOps
provider_slug: airops
slug: airops-domain-security
source_filename: airops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:57:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.airops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 09:11:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.airops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: airops.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/security/airops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applications
- AI
- Content
- SEO
- AEO
- Answer Engine Optimization
- Generative Engine Optimization
- Workflows
- MCP
- Analytics
---
