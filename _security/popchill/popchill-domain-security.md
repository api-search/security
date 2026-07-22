---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: popchill.com
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: popchill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Popchill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PopChill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PopChill
provider_slug: popchill
slug: popchill-domain-security
source_filename: popchill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: popchill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: popchill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popchill/refs/heads/main/security/popchill-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ecommerce
- Marketplace
- Fashion
- Secondhand
- Luxury Resale
- Mobile App
- Taiwan
---
