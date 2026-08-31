---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infineon.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.infineon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cypress Semiconductor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cypress Semiconductor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cypress Semiconductor
provider_slug: cypress-semiconductor
slug: cypress-semiconductor-domain-security
source_filename: cypress-semiconductor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infineon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: infineon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cypress-semiconductor/refs/heads/main/security/cypress-semiconductor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Acquired
- Bluetooth
- CapSense
- Embedded Systems
- Hardware
- Infineon
- IoT
- Microcontrollers
- NOR Flash
- PSoC
- Semiconductor
- WiFi
---
