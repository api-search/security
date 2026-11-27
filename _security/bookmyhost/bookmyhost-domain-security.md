---
api_specs:
- filename: bookmyhost-public-openapi.json
  format: json
  label: BookMyHost API
  slug: bookmyhost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bookmyhost/openapi/_original/bookmyhost-public-openapi.json
- filename: openapi.json
  format: json
  label: BookMyHost AI API (LiteLLM proxy)
  slug: bookmyhost-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bookmyhost/openapi/_original/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bookmyhost.com
  spf: true
hosts:
- cert_expires: Jan  6 11:32:59 2027 GMT
  host: bookmyhost.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 11:32:59 2027 GMT
  host: my.bookmyhost.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Blazing Bullet Private Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blazing Bullet Private Limited, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blazing Bullet Private Limited
provider_slug: bookmyhost
slug: bookmyhost-domain-security
source_filename: bookmyhost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bookmyhost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 11:32:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: my.bookmyhost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 11:32:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bookmyhost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bookmyhost/security/bookmyhost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Hosting
- VPS
- India
---
