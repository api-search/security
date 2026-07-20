---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dinmo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dinmo.io
  spf: true
hosts:
- cert_expires: Sep  5 19:33:56 2026 GMT
  host: www.dinmo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 10:36:10 2026 GMT
  host: docs.dinmo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 22:50:30 2026 GMT
  host: data-export-api.dinmo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dinmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DinMo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DinMo
provider_slug: dinmo
slug: dinmo-domain-security
source_filename: dinmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dinmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:33:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dinmo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:36:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data-export-api.dinmo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:50:30 2026 GMT\n  hsts: null\ndomains:\n- domain: dinmo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dinmo.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dinmo/refs/heads/main/security/dinmo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Customer Data Platform
- CDP
- Reverse ETL
- Data Activation
- Data Warehouse
- Audience Segmentation
- Marketing
- Personalization
- MarTech
---
