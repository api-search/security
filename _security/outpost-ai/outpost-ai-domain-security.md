---
api_specs:
- filename: outpost-ai-oauth-api-openapi.yml
  format: yaml
  label: Outpost OAuth API
  slug: outpost-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-oauth-api-openapi.yml
- filename: outpost-ai-payments-api-openapi.yml
  format: yaml
  label: Outpost Payments API
  slug: outpost-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-payments-api-openapi.yml
- filename: outpost-ai-webhooks-api-openapi.yml
  format: yaml
  label: Outpost Webhooks API
  slug: outpost-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: outpost.ai
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: outpost.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Outpost Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outpost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Outpost
provider_slug: outpost-ai
slug: outpost-ai-domain-security
source_filename: outpost-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outpost.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: outpost.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/outpost-ai/security/outpost-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Tax
- Commerce
- SaaS
---
