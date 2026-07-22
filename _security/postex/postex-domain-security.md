---
api_specs:
- filename: postex-order-openapi.yml
  format: yaml
  label: PostEx Merchant Order Integration API
  slug: postex-merchant-order-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postex/refs/heads/main/openapi/postex-order-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postex.pk
  spf: true
hosts:
- cert_expires: Oct  1 15:29:23 2026 GMT
  host: postex.pk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 15:29:23 2026 GMT
  host: api.postex.pk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostEx, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PostEx
provider_slug: postex
slug: postex-domain-security
source_filename: postex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postex.pk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:29:23 2026 GMT\n  hsts: false\n- host: api.postex.pk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:29:23 2026 GMT\n  hsts: null\ndomains:\n- domain: postex.pk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postex/refs/heads/main/security/postex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Courier
- Shipping
- E-commerce
- Fulfillment
- Cash on Delivery
- Payments
- Fintech
- Pakistan
---
