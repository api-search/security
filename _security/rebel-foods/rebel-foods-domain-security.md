---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rebelfoods.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eatsure.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.rebelfoods.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.eatsure.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rebel Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rebel Foods, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rebel Foods
provider_slug: rebel-foods
slug: rebel-foods-domain-security
source_filename: rebel-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rebelfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n- host: www.eatsure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: rebelfoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: eatsure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnote: www.eatsure.com is the consumer ordering platform Rebel Foods operates for its own brands; it was\n  probed with the same live DNS/TLS/HTTP checks and added by hand because apis.yml carries no apis[] entry\n  for it. Neither registrable domain publishes DNSSEC or CAA. rebelfoods.com serves no HSTS header; eatsure.com\n  does (max-age 15552000, includeSubDomains). eatsure.com DMARC\
  \ is p=none with aggregate/forensic reports\n  routed to consumer gmail.com mailboxes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rebel-foods/refs/heads/main/security/rebel-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Restaurant
- Cloud Kitchens
- Food Delivery
- Consumer
- Logistics
- India
---
