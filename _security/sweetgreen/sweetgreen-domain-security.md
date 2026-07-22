---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sweetgreen.com
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: www.sweetgreen.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sweetgreen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sweetgreen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sweetgreen
provider_slug: sweetgreen
slug: sweetgreen-domain-security
source_filename: sweetgreen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sweetgreen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sweetgreen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sweetgreen/refs/heads/main/security/sweetgreen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food
- Restaurants
- Food Delivery
- Loyalty
- Consumer
- Retail
---
