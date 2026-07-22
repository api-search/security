---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firstclub.site
  spf: false
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.firstclub.site
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: First Club
provider_slug: first-club
slug: first-club-domain-security
source_filename: first-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstclub.site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: firstclub.site\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-club/refs/heads/main/security/first-club-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Grocery
- Quick Commerce
- E-Commerce
- Delivery
- Consumer
- India
- Retail
---
