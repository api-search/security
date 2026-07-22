---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mealsinminutes.co
  spf: true
hosts:
- cert_expires: Oct 16 13:08:32 2026 GMT
  host: mealsinminutes.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meals In Minutes Mim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meals In Minutes, MIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Meals In Minutes, MIM
provider_slug: meals-in-minutes-mim
slug: meals-in-minutes-mim-domain-security
source_filename: meals-in-minutes-mim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mealsinminutes.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 13:08:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: mealsinminutes.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meals-in-minutes-mim/refs/heads/main/security/meals-in-minutes-mim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Meal Delivery
- E-Commerce
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
---
