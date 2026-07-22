---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elliscoffee.com
  spf: true
hosts:
- cert_expires: Sep 23 20:00:23 2026 GMT
  host: www.elliscoffee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ellis Coffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ellis Coffee Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ellis Coffee Company
provider_slug: ellis-coffee
slug: ellis-coffee-domain-security
source_filename: ellis-coffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elliscoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:00:23 2026 GMT\n  hsts: false\ndomains:\n- domain: elliscoffee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellis-coffee/refs/heads/main/security/ellis-coffee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Coffee
- Beverage
- Foodservice
- Wholesale
- Hospitality
---
