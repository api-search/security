---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: platejoy.com
  spf: true
hosts:
- host: platejoy.com
  https: false
kind: domain-security
layout: security
method: probed
name: Platejoy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlateJoy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PlateJoy
provider_slug: platejoy
slug: platejoy-domain-security
source_filename: platejoy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platejoy.com\n  https: false\ndomains:\n- domain: platejoy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platejoy/refs/heads/main/security/platejoy-domain-security.yml
summary_line: DMARC
tags:
- Company
- Meal Planning
- Nutrition
- Recipes
- Health
- Food
- Grocery
- Subscription
- Consumer
---
