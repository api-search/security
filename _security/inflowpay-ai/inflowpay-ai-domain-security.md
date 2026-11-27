---
api_specs:
- filename: inflowpay-ai-openapi-generated.yml
  format: yaml
  label: InFlow API
  slug: inflowpay-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflowpay-ai/openapi/_ae-authored/inflowpay-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inflowpay.ai
  spf: true
hosts:
- cert_expires: Dec 21 09:42:46 2026 GMT
  host: inflowpay.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InFlow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InFlow
provider_slug: inflowpay-ai
slug: inflowpay-ai-domain-security
source_filename: inflowpay-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inflowpay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:42:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inflowpay.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/inflowpay-ai/security/inflowpay-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Artificial Intelligence
- Fintech
- Commerce
- Automation
- Company
---
