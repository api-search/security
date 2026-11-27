---
api_specs:
- filename: reg-bot-ai-openapi-generated.yml
  format: yaml
  label: Regzy API
  slug: reg-bot-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reg-bot-ai/openapi/_ae-authored/reg-bot-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: reg-bot.ai
  spf: true
hosts:
- cert_expires: Jan  3 10:17:53 2027 GMT
  host: reg-bot.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Regzy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regzy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Regzy
provider_slug: reg-bot-ai
slug: reg-bot-ai-domain-security
source_filename: reg-bot-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reg-bot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 10:17:53 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: reg-bot.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reg-bot-ai/security/reg-bot-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- AI
- Small Business
- Security
- Integrity
---
