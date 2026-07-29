---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sydneyairport.com.au
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.sydneyairport.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sydney Airport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sydney Airport, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sydney Airport
provider_slug: sydney-airport
slug: sydney-airport-domain-security
source_filename: sydney-airport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sydneyairport.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sydneyairport.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sydney-airport/refs/heads/main/security/sydney-airport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Australia
- Airports
- Aviation
- Airport Infrastructure
- Transportation
- Flight Information
- Passenger Experience
---
