---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: foodology.com.co
  spf: true
hosts:
- cert_expires: Sep 24 22:17:13 2026 GMT
  host: www.foodology.com.co
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Foodology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foodology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Foodology
provider_slug: foodology
slug: foodology-domain-security
source_filename: foodology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foodology.com.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:17:13 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: foodology.com.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foodology/refs/heads/main/security/foodology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food Delivery
- Cloud Kitchen
- Virtual Restaurants
- Food Tech
- Latin America
- Consumer
---
