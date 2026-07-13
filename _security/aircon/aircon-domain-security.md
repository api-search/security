---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:24 2026 GMT
  host: developers.home.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: smartdevicemanagement.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 16:21:16 2026 GMT
  host: www.ecobee.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aircon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aircon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aircon
provider_slug: aircon
slug: aircon-domain-security
source_filename: aircon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.home.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: smartdevicemanagement.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: www.ecobee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:21:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/security/aircon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Air Conditioning
- HVAC
- Climate Control
- IoT
- Smart Home
- Thermostat
- Building Automation
- Energy Management
---
