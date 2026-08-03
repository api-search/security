---
api_specs:
- filename: bolt-financial-bolt-api-openapi.yml
  format: yaml
  label: Bolt API
  slug: bolt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-bolt-api-openapi.yml
- filename: bolt-financial-embeddable-checkout-v1-openapi.yml
  format: yaml
  label: Bolt Embeddable Checkout v1 API
  slug: embeddable-checkout-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-embeddable-checkout-v1-openapi.yml
- filename: bolt-financial-embeddable-checkout-v3-openapi.yml
  format: yaml
  label: Bolt Embeddable Checkout v3 API
  slug: embeddable-checkout-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-embeddable-checkout-v3-openapi.yml
- filename: bolt-financial-tokenizer-openapi.yml
  format: yaml
  label: Bolt Tokenizer API
  slug: tokenizer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-tokenizer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bolt.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boltapp.com
  spf: true
hosts:
- cert_expires: Oct 12 14:53:16 2026 GMT
  host: www.bolt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 18:22:53 2026 GMT
  host: help.boltapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.boltapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bolt Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolt Financial, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bolt Financial
provider_slug: bolt-financial
slug: bolt-financial-domain-security
source_filename: bolt-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bolt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 14:53:16 2026 GMT\n  hsts: null\n- host: help.boltapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 18:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.boltapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bolt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: boltapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/security/bolt-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Checkout
- eCommerce
- Fintech
- Subscriptions
- Tokenization
- Fraud
- Identity
- Webhooks
---
