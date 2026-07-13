---
api_specs:
- filename: lemon-squeezy-api-openapi.yml
  format: yaml
  label: Lemon Squeezy API
  slug: lemon-squeezy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemon-squeezy/refs/heads/main/openapi/lemon-squeezy-api-openapi.yml
- filename: lemon-squeezy-license-api-openapi.yml
  format: yaml
  label: Lemon Squeezy License API
  slug: lemon-squeezy-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemon-squeezy/refs/heads/main/openapi/lemon-squeezy-license-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lemonsqueezy.com
  spf: true
hosts:
- cert_expires: Oct  6 09:03:07 2026 GMT
  host: www.lemonsqueezy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 09:03:07 2026 GMT
  host: docs.lemonsqueezy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 09:03:07 2026 GMT
  host: api.lemonsqueezy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemon Squeezy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemon Squeezy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lemon Squeezy
provider_slug: lemon-squeezy
slug: lemon-squeezy-domain-security
source_filename: lemon-squeezy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lemonsqueezy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lemonsqueezy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lemonsqueezy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:03:07 2026 GMT\n  hsts: null\ndomains:\n- domain: lemonsqueezy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemon-squeezy/refs/heads/main/security/lemon-squeezy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Products
- Ecommerce
- Products
---
