---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sheetsu.com
  spf: false
hosts:
- cert_expires: Aug 22 02:40:13 2026 GMT
  host: sheetsu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sheetsu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sheetsu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sheetsu
provider_slug: sheetsu
slug: sheetsu-domain-security
source_filename: sheetsu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sheetsu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:40:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sheetsu.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sheetsu/refs/heads/main/security/sheetsu-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Development
- Public APIs
---
