---
api_specs:
- filename: moxion-power-co-openapi.yml
  format: yaml
  label: Moxion Power Developer API
  slug: moxion-power-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxion-power-co/refs/heads/main/openapi/moxion-power-co-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moxionpower.com
  spf: true
hosts:
- host: www.moxionpower.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- cert_expires: Oct  4 07:54:00 2026 GMT
  host: developer.moxionpower.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.moxionpower.com
  https: false
kind: domain-security
layout: security
method: probed
name: Moxion Power Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moxion Power Co, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Moxion Power Co
provider_slug: moxion-power-co
slug: moxion-power-co-domain-security
source_filename: moxion-power-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moxionpower.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: developer.moxionpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:54:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moxionpower.com\n  https: false\ndomains:\n- domain: moxionpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moxion-power-co/refs/heads/main/security/moxion-power-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy Storage
- Mobile Power
- Battery
- Telemetry
- IoT
- Fleet Management
- Clean Energy
- Construction
- Device Metrics
---
