---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: texel.live
  spf: true
hosts:
- cert_expires: Sep 22 11:13:44 2026 GMT
  host: texel.live
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Texel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Texel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Texel
provider_slug: texel
slug: texel-domain-security
source_filename: texel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: texel.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:13:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: texel.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texel/refs/heads/main/security/texel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
