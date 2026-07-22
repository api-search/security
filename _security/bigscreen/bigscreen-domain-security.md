---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bigscreenvr.com
  spf: false
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: www.bigscreenvr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bigscreen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BigScreen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: BigScreen
provider_slug: bigscreen
slug: bigscreen-domain-security
source_filename: bigscreen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bigscreenvr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bigscreenvr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigscreen/refs/heads/main/security/bigscreen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Virtual Reality
- VR
- Hardware
- Consumer Electronics
- Entertainment
- Headset
- Social VR
---
