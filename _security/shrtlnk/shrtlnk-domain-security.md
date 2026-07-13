---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shrtlnk.dev
  spf: true
hosts:
- cert_expires: Sep  8 04:29:16 2026 GMT
  host: shrtlnk.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shrtlnk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shrtlnk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shrtlnk
provider_slug: shrtlnk
slug: shrtlnk-domain-security
source_filename: shrtlnk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shrtlnk.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:29:16 2026 GMT\n  hsts: false\ndomains:\n- domain: shrtlnk.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shrtlnk/refs/heads/main/security/shrtlnk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- URL Shorteners
- Public APIs
---
