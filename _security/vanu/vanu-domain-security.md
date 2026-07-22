---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vanu.com
  spf: true
hosts:
- cert_expires: Sep  3 20:48:03 2026 GMT
  host: vanu.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vanu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vanu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vanu
provider_slug: vanu
slug: vanu-domain-security
source_filename: vanu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vanu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 20:48:03 2026 GMT\n  hsts: false\ndomains:\n- domain: vanu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanu/refs/heads/main/security/vanu-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Telecommunications
- Wireless
- Cellular Networks
- Rural Connectivity
- Software Defined Radio
- Network Infrastructure
- Coverage Mapping
---
