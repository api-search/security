---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nokia.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nokia.io
  spf: false
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.nokia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: network.developer.nokia.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: networkascode.nokia.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nokia Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nokia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nokia
provider_slug: nokia-corp
slug: nokia-corp-domain-security
source_filename: nokia-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nokia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: network.developer.nokia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\n- host: networkascode.nokia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nokia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nokia.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nokia-corp/refs/heads/main/security/nokia-corp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Telecom
- 5G
- 6G
- Mobile Networks
- Network Infrastructure
- IP Networks
- Optical Networks
- Fixed Networks
- Broadband
- Service Router
- SR OS
- SR Linux
- WaveSuite
- NSP
- Network Services Platform
- Network as Code
- CAMARA
- Network Exposure
- Open Gateway
- YANG
- Network Automation
- CSP
- Bell Labs
- Submarine Cable
- Fiber
- 7x50
---
