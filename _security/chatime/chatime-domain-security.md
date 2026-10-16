---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chatime.com.tw
  spf: true
hosts:
- cert_expires: Nov 15 13:01:50 2026 GMT
  host: www.chatime.com.tw
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chatime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chatime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chatime
provider_slug: chatime
slug: chatime-domain-security
source_filename: chatime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chatime.com.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 13:01:50 2026 GMT\n  hsts: false\ndomains:\n- domain: chatime.com.tw\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatime/refs/heads/main/security/chatime-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- BubbleTea
- Franchise
- Food&Beverage
- Global
---
