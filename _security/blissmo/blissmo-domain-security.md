---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blissmo.com
  spf: false
hosts:
- cert_expires: Jan 31 14:27:21 2027 GMT
  host: blissmo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blissmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blissmo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Blissmo
provider_slug: blissmo
slug: blissmo-domain-security
source_filename: blissmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blissmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 14:27:21 2027 GMT\n  hsts: null\ndomains:\n- domain: blissmo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blissmo/refs/heads/main/security/blissmo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
