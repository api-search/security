---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sedonasys.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: sedonasys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sedona Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sedona Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sedona Systems
provider_slug: sedona-systems
slug: sedona-systems-domain-security
source_filename: sedona-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sedonasys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sedonasys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sedona-systems/refs/heads/main/security/sedona-systems-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Deep Tech
- Networking
- Network Optimization
- Optical Networking
- Telecommunications
- Acquired
---
