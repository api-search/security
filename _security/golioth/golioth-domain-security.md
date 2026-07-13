---
api_specs:
- filename: golioth-openapi.yml
  format: yaml
  label: Golioth Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golioth/refs/heads/main/openapi/golioth-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: golioth.io
  spf: true
hosts:
- cert_expires: Aug 16 07:00:03 2026 GMT
  host: golioth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 09:23:56 2026 GMT
  host: docs.golioth.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 14:05:49 2026 GMT
  host: api.golioth.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Golioth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golioth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Golioth
provider_slug: golioth
slug: golioth-domain-security
source_filename: golioth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: golioth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:00:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.golioth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 09:23:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.golioth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:05:49 2026 GMT\n  hsts: null\ndomains:\n- domain: golioth.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golioth/refs/heads/main/security/golioth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Device Management
- Firmware
- Zephyr
- OTA
- Embedded
- Connectivity
---
