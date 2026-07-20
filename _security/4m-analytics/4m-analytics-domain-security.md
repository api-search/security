---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 4manalytics.com
  spf: false
hosts:
- cert_expires: Oct  3 15:23:12 2026 GMT
  host: www.4manalytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 16:44:23 2026 GMT
  host: help.4manalytics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 4M Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4M Analytics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: 4M Analytics
provider_slug: 4m-analytics
slug: 4m-analytics-domain-security
source_filename: 4m-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.4manalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:23:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.4manalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 16:44:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: 4manalytics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4m-analytics/refs/heads/main/security/4m-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Geospatial
- GIS
- Mapping
- Utilities
- Infrastructure
- Subsurface
- Location Intelligence
- AI
- Construction Technology
---
