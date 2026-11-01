---
api_specs:
- filename: meal-planner-online.openapi.json
  format: json
  label: Meal Planner Read-only API
  slug: meal-planner-read-only-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meal-planner-online/openapi/meal-planner-online.openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meal-planner.online
  spf: true
hosts:
- cert_expires: Jan 25 02:28:54 2027 GMT
  host: meal-planner.online
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meal Planner Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for meal-planner-online, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: meal-planner-online
provider_slug: meal-planner-online
slug: meal-planner-online-domain-security
source_filename: meal-planner-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meal-planner.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 02:28:54 2027 GMT\n  hsts: false\ndomains:\n- domain: meal-planner.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/meal-planner-online/security/meal-planner-online-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Meal Planning
- Family
- Canada
- API
- Subscription
- Cooking
---
