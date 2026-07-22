---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zo.computer
  spf: false
hosts:
- cert_expires: Sep  8 13:02:47 2026 GMT
  host: api.zo.computer
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zocomputer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zocomputer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Zocomputer
provider_slug: zocomputer
slug: zocomputer-domain-security
source_filename: zocomputer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.zo.computer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 13:02:47 2026 GMT\n  hsts: null\ndomains:\n- domain: zo.computer\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zocomputer/refs/heads/main/security/zocomputer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
