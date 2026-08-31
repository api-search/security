---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wecasa.fr
  spf: true
hosts:
- cert_expires: Oct 29 08:03:43 2026 GMT
  host: www.wecasa.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wecasa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wecasa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wecasa
provider_slug: wecasa
slug: wecasa-domain-security
source_filename: wecasa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wecasa.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 08:03:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wecasa.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wecasa/refs/heads/main/security/wecasa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Marketplace
- Home Services
- Beauty and Wellness
- Cleaning
- Childcare
- On Demand
- France
- Mobile Apps
---
