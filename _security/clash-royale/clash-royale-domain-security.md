---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clashroyale.com
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: developer.clashroyale.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clash Royale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clash Royale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Clash Royale
provider_slug: clash-royale
slug: clash-royale-domain-security
source_filename: clash-royale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.clashroyale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: clashroyale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clash-royale/refs/heads/main/security/clash-royale-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
