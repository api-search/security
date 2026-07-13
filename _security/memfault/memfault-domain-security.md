---
api_specs:
- filename: memfault-openapi.yml
  format: yaml
  label: Memfault Cloud REST API
  slug: memfault-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: memfault.com
  spf: true
hosts:
- cert_expires: Sep 14 06:01:51 2026 GMT
  host: memfault.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 19:12:57 2026 GMT
  host: api-docs.memfault.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: api.memfault.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memfault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memfault, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Memfault
provider_slug: memfault
slug: memfault-domain-security
source_filename: memfault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memfault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.memfault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:12:57 2026 GMT\n  hsts: false\n- host: api.memfault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: memfault.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/security/memfault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alerts
- Android
- Crash Reporting
- Device Management
- Embedded
- Embedded Linux
- Firmware
- IoT
- Logging
- MCU
- Metrics
- Observability
- OTA
- Reliability
---
