---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: foodadvisor.my
  spf: false
hosts:
- cert_expires: Oct  8 03:04:30 2026 GMT
  host: foodadvisor.my
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Food Advisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Food Advisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Food Advisor
provider_slug: food-advisor
slug: food-advisor-domain-security
source_filename: food-advisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foodadvisor.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:04:30 2026 GMT\n  hsts: null\ndomains:\n- domain: foodadvisor.my\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/food-advisor/refs/heads/main/security/food-advisor-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Food
- Food Discovery
- Restaurants
- Mobile App
- Malaysia
- Startup
---
