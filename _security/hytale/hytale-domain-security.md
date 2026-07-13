---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hytale-api.com
  spf: false
hosts:
- cert_expires: Aug 17 19:02:29 2026 GMT
  host: hytale-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hytale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hytale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hytale
provider_slug: hytale
slug: hytale-domain-security
source_filename: hytale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hytale-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:02:29 2026 GMT\n  hsts: null\ndomains:\n- domain: hytale-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hytale/refs/heads/main/security/hytale-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
