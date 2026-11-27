---
api_specs:
- filename: lenius-app-butikker-api-openapi.yml
  format: yaml
  label: lenius-app Butikker API
  slug: lenius-app-butikker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenius-app/openapi/lenius-app-butikker-api-openapi.yml
- filename: lenius-app-butikskategorier-api-openapi.yml
  format: yaml
  label: lenius-app Butikskategorier API
  slug: lenius-app-butikskategorier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenius-app/openapi/lenius-app-butikskategorier-api-openapi.yml
- filename: lenius-app-system-api-openapi.yml
  format: yaml
  label: lenius-app System API
  slug: lenius-app-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenius-app/openapi/lenius-app-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lenius.app
  spf: true
hosts:
- host: lenius.app
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: lenius-app Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lenius-app, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: lenius-app
provider_slug: lenius-app
slug: lenius-app-domain-security
source_filename: lenius-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lenius.app\n  https: false\ndomains:\n- domain: lenius.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lenius-app/security/lenius-app-domain-security.yml
summary_line: DMARC
tags:
- Company
---
