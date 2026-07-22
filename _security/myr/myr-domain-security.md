---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myr.io
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: myr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MYR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MYR
provider_slug: myr
slug: myr-domain-security
source_filename: myr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: myr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myr/refs/heads/main/security/myr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Point of Sale
- Restaurants
- Quick Service Restaurants
- Food Service Technology
- Payments
- Loyalty
- Restaurant Management
- Integrations
---
