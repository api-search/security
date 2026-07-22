---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wi-charge.com
  spf: true
hosts:
- cert_expires: Aug 28 12:02:48 2026 GMT
  host: wi-charge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wi Charge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wi Charge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wi Charge
provider_slug: wi-charge
slug: wi-charge-domain-security
source_filename: wi-charge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wi-charge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:02:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wi-charge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wi-charge/refs/heads/main/security/wi-charge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wireless Power
- Wireless Charging
- Infrared
- IoT
- Smart Home
- Hardware
- OEM
- Consumer Electronics
- Energy
---
