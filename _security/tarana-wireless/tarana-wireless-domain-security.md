---
api_specs:
- filename: tarana-wireless-alerts-asyncapi.yml
  format: yaml
  label: Tarana Cloud Suite (TCS) Northbound API
  slug: tarana-cloud-suite-tcs-northbound-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tarana-wireless/refs/heads/main/asyncapi/tarana-wireless-alerts-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: taranawireless.com
  spf: true
hosts:
- cert_expires: Nov  4 01:47:00 2026 GMT
  host: www.taranawireless.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: portal.tcs.taranawireless.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tarana Wireless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tarana Wireless, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tarana Wireless
provider_slug: tarana-wireless
slug: tarana-wireless-domain-security
source_filename: tarana-wireless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.taranawireless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 01:47:00 2026 GMT\n  hsts: null\n- host: portal.tcs.taranawireless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: taranawireless.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tarana-wireless/refs/heads/main/security/tarana-wireless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Networking
- Telecommunications
- Fixed Wireless Access
- Broadband
- Wireless
- Network Management
- Internet Service Providers
- CBRS
- Spectrum
- Telemetry
- Hardware
---
