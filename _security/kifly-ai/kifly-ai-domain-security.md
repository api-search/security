---
api_specs:
- filename: kifly-ai-openapi-generated.yml
  format: yaml
  label: Kifly API
  slug: kifly-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kifly-ai/openapi/_ae-authored/kifly-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kifly.ai
  spf: true
hosts:
- cert_expires: Jan  5 16:04:07 2027 GMT
  host: kifly.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kifly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kifly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kifly
provider_slug: kifly-ai
slug: kifly-ai-domain-security
source_filename: kifly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kifly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 16:04:07 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kifly.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kifly-ai/security/kifly-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Commerce
- Catalog Integration
- Shopify
- WooCommerce
- Agent Checkout
- Payments
- AI Agents
---
