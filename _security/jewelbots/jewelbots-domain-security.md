---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jewelbots.com
  spf: false
hosts:
- cert_expires: Aug 28 03:19:02 2026 GMT
  host: jewelbots.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jewelbots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jewelbots, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jewelbots
provider_slug: jewelbots
slug: jewelbots-domain-security
source_filename: jewelbots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jewelbots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 03:19:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: jewelbots.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jewelbots/refs/heads/main/security/jewelbots-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Wearables
- Hardware
- IoT
- Bluetooth
- Arduino
- Firmware
- Education
- Open Source
---
