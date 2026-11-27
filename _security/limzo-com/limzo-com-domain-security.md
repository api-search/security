---
api_specs:
- filename: limzo-com-public-api-openapi.yml
  format: yaml
  label: Limzo Public API
  slug: limzo-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/limzo-com/openapi/limzo-com-public-api-openapi.yml
- filename: limzo-com-s-api-openapi.yml
  format: yaml
  label: Limzo S API
  slug: limzo-com-s-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/limzo-com/openapi/limzo-com-s-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: limzo.com
  spf: true
hosts:
- cert_expires: Jan 23 09:05:21 2027 GMT
  host: limzo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Limzo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Limzo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Limzo
provider_slug: limzo-com
slug: limzo-com-domain-security
source_filename: limzo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: limzo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 09:05:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: limzo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/limzo-com/security/limzo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telegram
- Bot
- Anti-Spam
- Group Analytics
---
