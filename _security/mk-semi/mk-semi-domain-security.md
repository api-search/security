---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mk-semi.com
  spf: false
hosts:
- cert_expires: Oct 16 04:08:20 2026 GMT
  host: mk-semi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mk Semi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mauna Kea Semiconductors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mauna Kea Semiconductors
provider_slug: mk-semi
slug: mk-semi-domain-security
source_filename: mk-semi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mk-semi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 04:08:20 2026 GMT\n  hsts: false\ndomains:\n- domain: mk-semi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mk-semi/refs/heads/main/security/mk-semi-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Semiconductors
- Ultra-Wideband
- UWB
- Hardware
- Chips
- IoT
- Positioning
---
