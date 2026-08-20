---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nex.ad
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: soku.ai
  spf: true
hosts:
- cert_expires: Nov  6 14:47:16 2026 GMT
  host: nex.ad
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 03:10:58 2026 GMT
  host: docs.nex.ad
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 22:46:07 2026 GMT
  host: soku.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexad, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nexad
provider_slug: nexad
slug: nexad-domain-security
source_filename: nexad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nex.ad\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 14:47:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nex.ad\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:10:58 2026 GMT\n  hsts: false\n- host: soku.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 22:46:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nex.ad\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: soku.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexad/refs/heads/main/security/nexad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Advertising
- Marketing
- Marketing Automation
- Contextual Advertising
- Mobile SDK
- Agents
---
