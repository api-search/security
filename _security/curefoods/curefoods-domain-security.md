---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: curefoods.in
  spf: true
hosts:
- cert_expires: Sep 21 15:27:47 2026 GMT
  host: curefoods.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curefoods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curefoods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Curefoods
provider_slug: curefoods
slug: curefoods-domain-security
source_filename: curefoods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curefoods.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:27:47 2026 GMT\n  hsts: false\ndomains:\n- domain: curefoods.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curefoods/refs/heads/main/security/curefoods-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Food and Beverage
- Cloud Kitchen
- Restaurants
- Food Delivery
- India
---
