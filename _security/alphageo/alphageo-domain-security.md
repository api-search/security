---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alphageo.ai
  spf: true
hosts:
- cert_expires: Aug 29 12:43:08 2026 GMT
  host: alphageo.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:40:21 2026 GMT
  host: docs.alphageo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: app.alphageo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alphageo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alphageo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alphageo
provider_slug: alphageo
slug: alphageo-domain-security
source_filename: alphageo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alphageo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 12:43:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.alphageo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:40:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.alphageo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alphageo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphageo/refs/heads/main/security/alphageo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate
- Climate Risk
- Geospatial
- Analytics
- Risk
- Real Estate
- ESG
- Data
- Machine Learning
---
