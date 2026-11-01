---
api_specs:
- filename: bettermenu-conversions-api-openapi.yml
  format: yaml
  label: BetterMenu Conversions API
  slug: bettermenu-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bettermenu/openapi/bettermenu-conversions-api-openapi.yml
- filename: bettermenu-entitlements-api-openapi.yml
  format: yaml
  label: BetterMenu Entitlements API
  slug: bettermenu-entitlements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bettermenu/openapi/bettermenu-entitlements-api-openapi.yml
- filename: bettermenu-org-api-openapi.yml
  format: yaml
  label: BetterMenu Org API
  slug: bettermenu-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bettermenu/openapi/bettermenu-org-api-openapi.yml
- filename: bettermenu-studio-api-openapi.yml
  format: yaml
  label: BetterMenu Studio API
  slug: bettermenu-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bettermenu/openapi/bettermenu-studio-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bettermenu.live
  spf: true
hosts:
- cert_expires: Jan 12 21:29:57 2027 GMT
  host: bettermenu.live
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bettermenu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetterMenu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BetterMenu
provider_slug: bettermenu
slug: bettermenu-domain-security
source_filename: bettermenu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bettermenu.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 21:29:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: bettermenu.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bettermenu/security/bettermenu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FoodTech
- RecipeFormulation
- FDACompliance
- SaaS
- Cloud
---
