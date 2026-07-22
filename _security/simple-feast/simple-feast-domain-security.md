---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: simplefeast.com
  spf: false
hosts:
- host: food.simplefeast.com
  https: false
kind: domain-security
layout: security
method: probed
name: Simple Feast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simple Feast, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Simple Feast
provider_slug: simple-feast
slug: simple-feast-domain-security
source_filename: simple-feast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: food.simplefeast.com\n  https: false\ndomains:\n- domain: simplefeast.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simple-feast/refs/heads/main/security/simple-feast-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Food
- Meal Kit
- Meal Delivery
- Plant-Based
- E-Commerce
---
