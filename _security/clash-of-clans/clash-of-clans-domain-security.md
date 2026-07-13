---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clashofclans.com
  spf: false
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: developer.clashofclans.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clash Of Clans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clash of Clans, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Clash of Clans
provider_slug: clash-of-clans
slug: clash-of-clans-domain-security
source_filename: clash-of-clans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.clashofclans.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: clashofclans.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clash-of-clans/refs/heads/main/security/clash-of-clans-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
