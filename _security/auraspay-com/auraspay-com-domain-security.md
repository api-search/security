---
api_specs:
- filename: auraspay-com-account-api-openapi.yml
  format: yaml
  label: AurasPay Account API
  slug: auraspay-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-account-api-openapi.yml
- filename: auraspay-com-agent-checkout-api-openapi.yml
  format: yaml
  label: AurasPay Agent Checkout API
  slug: auraspay-com-agent-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-agent-checkout-api-openapi.yml
- filename: auraspay-com-payment-links-api-openapi.yml
  format: yaml
  label: AurasPay Payment Links API
  slug: auraspay-com-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-payment-links-api-openapi.yml
- filename: auraspay-com-supported-tokens-api-openapi.yml
  format: yaml
  label: AurasPay Supported Tokens API
  slug: auraspay-com-supported-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-supported-tokens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: auraspay.com
  spf: true
hosts:
- cert_expires: Jan 19 19:15:10 2027 GMT
  host: auraspay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auraspay Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AurasPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AurasPay
provider_slug: auraspay-com
slug: auraspay-com-domain-security
source_filename: auraspay-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auraspay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 19:15:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: auraspay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/auraspay-com/security/auraspay-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Cryptocurrency
- Stablecoins
---
