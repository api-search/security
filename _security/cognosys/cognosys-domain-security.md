---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cognosys.ai
  spf: false
hosts:
- cert_expires: Sep 15 07:49:08 2026 GMT
  host: cognosys.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognosys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognosys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cognosys
provider_slug: cognosys
slug: cognosys-domain-security
source_filename: cognosys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognosys.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:49:08 2026 GMT\n  hsts: null\ndomains:\n- domain: cognosys.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognosys/refs/heads/main/security/cognosys-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
---
