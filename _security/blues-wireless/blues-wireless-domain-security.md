---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Notehub API
  slug: blues-wireless-notehub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/blues/notehub-js/main/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blues.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blues.io
  spf: true
hosts:
- cert_expires: Aug 19 14:56:10 2026 GMT
  host: blues.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: dev.blues.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.notefile.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blues Wireless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blues, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blues
provider_slug: blues-wireless
slug: blues-wireless-domain-security
source_filename: blues-wireless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blues.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:56:10 2026 GMT\n  hsts: false\n- host: dev.blues.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\n- host: api.notefile.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: blues.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: blues.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/security/blues-wireless-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- IoT
- Cellular
- Connectivity
- Device Management
- Fleet Management
- Satellite
- LoRa
- WiFi
- Notecard
- Notehub
---
