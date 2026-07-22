---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bluage.co.jp
  spf: true
hosts:
- cert_expires: Aug 29 14:57:15 2026 GMT
  host: bluage.co.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BluAge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BluAge
provider_slug: bluage
slug: bluage-domain-security
source_filename: bluage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluage.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 14:57:15 2026 GMT\n  hsts: null\ndomains:\n- domain: bluage.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluage/refs/heads/main/security/bluage-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
