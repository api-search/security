---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rentify.com
  spf: true
hosts:
- cert_expires: Aug 25 06:20:25 2026 GMT
  host: www.rentify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rentify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: rentify
provider_slug: rentify
slug: rentify-domain-security
source_filename: rentify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rentify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 06:20:25 2026 GMT\n  hsts: null\ndomains:\n- domain: rentify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentify/refs/heads/main/security/rentify-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- PropTech
- Real Estate
- Property Management
- Lettings
- Rental
- United Kingdom
---
