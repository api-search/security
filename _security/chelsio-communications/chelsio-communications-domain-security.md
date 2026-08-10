---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chelsio.com
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.chelsio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chelsio Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chelsio Communications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chelsio Communications
provider_slug: chelsio-communications
slug: chelsio-communications-domain-security
source_filename: chelsio-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chelsio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chelsio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chelsio-communications/refs/heads/main/security/chelsio-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Networking
- Hardware
- Semiconductors
- Ethernet
- Storage
- RDMA
- Data Center
- Drivers
---
