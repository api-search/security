---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: butlr.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: butlr.io
  spf: true
hosts:
- cert_expires: Aug 19 07:16:20 2026 GMT
  host: butlr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 21:26:06 2026 GMT
  host: docs.butlr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.butlr.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Butlr Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Butlr Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Butlr Technologies
provider_slug: butlr-technologies
slug: butlr-technologies-domain-security
source_filename: butlr-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: butlr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:16:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.butlr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:26:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.butlr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: butlr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: butlr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butlr-technologies/refs/heads/main/security/butlr-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Occupancy Sensing
- People Counting
- Smart Buildings
- Space Utilization
- IoT
- Thermal Sensors
- Real-Time Data
- GraphQL
- Webhooks
---
