---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ypxfood.com
  spf: false
hosts:
- cert_expires: Sep 24 15:28:55 2026 GMT
  host: ypxfood.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ypxfood Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ypxfood, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ypxfood
provider_slug: ypxfood
slug: ypxfood-domain-security
source_filename: ypxfood-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ypxfood.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:28:55 2026 GMT\n  hsts: null\ndomains:\n- domain: ypxfood.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ypxfood/refs/heads/main/security/ypxfood-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Food
- Restaurant
- Quick Service Restaurant
- Taiwan
---
