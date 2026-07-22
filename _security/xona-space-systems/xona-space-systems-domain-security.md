---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xonaspace.com
  spf: true
hosts:
- cert_expires: Oct  3 23:52:24 2026 GMT
  host: xonaspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xona Space Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xona Space Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xona Space Systems
provider_slug: xona-space-systems
slug: xona-space-systems-domain-security
source_filename: xona-space-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xonaspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:52:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xonaspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xona-space-systems/refs/heads/main/security/xona-space-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Frontier Tech
- Space
- Satellites
- Navigation
- PNT
- Timing
- LEO
---
