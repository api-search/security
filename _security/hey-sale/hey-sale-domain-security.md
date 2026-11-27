---
api_specs:
- filename: hey-sale-openapi-generated.yml
  format: yaml
  label: HeySale API
  slug: hey-sale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hey-sale/openapi/_ae-authored/hey-sale-openapi-generated.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hey.sale
  spf: true
hosts:
- cert_expires: Jan  3 19:58:00 2027 GMT
  host: hey.sale
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HeySale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeySale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HeySale
provider_slug: hey-sale
slug: hey-sale-domain-security
source_filename: hey-sale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hey.sale\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 19:58:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hey.sale\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hey-sale/security/hey-sale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Sales Automation
- Conversational AI
- B2B
- Software-as-a-Service
---
