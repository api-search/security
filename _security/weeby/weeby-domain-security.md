---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gameclosure.com
  spf: true
hosts:
- cert_expires: Oct 15 02:59:00 2026 GMT
  host: gameclosure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weeby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weeby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Weeby
provider_slug: weeby
slug: weeby-domain-security
source_filename: weeby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gameclosure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:59:00 2026 GMT\n  hsts: false\ndomains:\n- domain: gameclosure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weeby/refs/heads/main/security/weeby-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Gaming
- Mobile Games
- Social Games
- Portfolio Company
- 500 Global
---
