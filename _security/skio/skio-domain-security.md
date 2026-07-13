---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skio.com
  spf: true
hosts:
- cert_expires: Sep  6 15:01:54 2026 GMT
  host: skio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: code.skio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 02:56:23 2026 GMT
  host: graphql.skio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skio
provider_slug: skio
slug: skio-domain-security
source_filename: skio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:01:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: code.skio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n- host: graphql.skio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:56:23 2026 GMT\n  hsts: null\ndomains:\n- domain: skio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skio/refs/heads/main/security/skio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Subscriptions
- Shopify
- Ecommerce
- DTC
- Recurring Billing
- GraphQL
---
