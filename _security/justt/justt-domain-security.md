---
api_specs:
- filename: justt-rest-api-openapi-original.json
  format: json
  label: Justt REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-rest-api-openapi-original.json
- filename: justt-pre-chargeback-alerts-openapi-original.json
  format: json
  label: Justt Pre-Chargeback Alerts API
  slug: pre-chargeback-alerts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-pre-chargeback-alerts-openapi-original.json
- filename: justt-webhook-events-openapi-original.json
  format: json
  label: Justt Webhook Events
  slug: webhook-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/asyncapi/justt-webhook-events-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: justt.ai
  spf: true
hosts:
- cert_expires: Oct 29 06:19:50 2026 GMT
  host: justt.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 12:18:20 2026 GMT
  host: developers.justt.ai
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 14:36:51 2026 GMT
  host: api.justt.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Justt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Justt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Justt
provider_slug: justt
slug: justt-domain-security
source_filename: justt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 06:19:50 2026 GMT\n  hsts: false\n- host: developers.justt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 12:18:20 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: api.justt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 14:36:51 2026 GMT\n  hsts: null\ndomains:\n- domain: justt.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/security/justt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Chargebacks
- Disputes
- Fraud
- Risk
- Financial Services
- E-Commerce
- Artificial Intelligence
- Webhooks
---
