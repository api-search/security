---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: proemion.com
  spf: true
hosts:
- cert_expires: Aug 25 12:51:15 2026 GMT
  host: www.proemion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: docs.proemion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: api.proemion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proemion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proemion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Proemion
provider_slug: proemion
slug: proemion-domain-security
source_filename: proemion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proemion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:51:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.proemion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.proemion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: proemion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proemion/refs/heads/main/security/proemion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Telematics
- IoT
- Off-Highway Equipment
- CAN Bus
- Fleet Management
- Machine Data
- OEM
- AEMP
- Construction
- Agriculture
---
