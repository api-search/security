---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: accelercomm.com
  spf: true
hosts:
- cert_expires: Nov 12 17:12:51 2026 GMT
  host: www.accelercomm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accelercomm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AccelerComm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AccelerComm
provider_slug: accelercomm
slug: accelercomm-domain-security
source_filename: accelercomm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accelercomm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 17:12:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: accelercomm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelercomm/refs/heads/main/security/accelercomm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Semiconductor IP
- Telecommunications
- Wireless
- 5G
- Non-Terrestrial Networks
- Satellite Communications
- Channel Coding
- Forward Error Correction
- Physical Layer
- Radio Access Networks
- FPGA
- United Kingdom
---
