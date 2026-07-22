---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mealplanet.com
  spf: true
hosts:
- cert_expires: Oct 17 09:53:23 2026 GMT
  host: mealplanet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meal Planet Holding Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MEAL PLANET HOLDING LTD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MEAL PLANET HOLDING LTD
provider_slug: meal-planet-holding-ltd
slug: meal-planet-holding-ltd-domain-security
source_filename: meal-planet-holding-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mealplanet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 09:53:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mealplanet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meal-planet-holding-ltd/refs/heads/main/security/meal-planet-holding-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Foodtech
- Meal Delivery
- Meal Plans
- Marketplace
- Subscription
- Consumer App
- UAE
- Food
---
