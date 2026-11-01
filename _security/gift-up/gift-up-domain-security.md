---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: giftup.com
  spf: true
hosts:
- cert_expires: Jan 14 20:55:49 2027 GMT
  host: giftup.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gift Up Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gift Up!, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gift Up!
provider_slug: gift-up
slug: gift-up-domain-security
source_filename: gift-up-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: giftup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 20:55:49 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: giftup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gift-up/security/gift-up-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- E-commerce
- Gift Cards
- SaaS
---
