---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crossbar-inc.com
  spf: true
hosts:
- cert_expires: Sep 23 16:56:30 2026 GMT
  host: www.crossbar-inc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crossbar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossbar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crossbar
provider_slug: crossbar
slug: crossbar-domain-security
source_filename: crossbar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossbar-inc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:56:30 2026 GMT\n  hsts: null\ndomains:\n- domain: crossbar-inc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossbar/refs/heads/main/security/crossbar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hardtech
- Semiconductors
- Memory
- ReRAM
- Storage
- IoT
---
