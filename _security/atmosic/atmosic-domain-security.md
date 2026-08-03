---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atmosic.com
  spf: true
hosts:
- cert_expires: Sep 28 00:07:49 2026 GMT
  host: atmosic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atmosic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmosic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atmosic
provider_slug: atmosic
slug: atmosic-domain-security
source_filename: atmosic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atmosic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:07:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atmosic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmosic/refs/heads/main/security/atmosic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Bluetooth Low Energy
- Wireless
- Energy Harvesting
- IoT
- Embedded Systems
- System on Chip
- Zephyr RTOS
- Low Power
- Hardware
---
