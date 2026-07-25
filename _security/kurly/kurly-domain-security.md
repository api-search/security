---
api_specs:
- filename: kurly-authentication-api-openapi.yml
  format: yaml
  label: Kurly Authentication API
  slug: kurly-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-authentication-api-openapi.yml
- filename: kurly-default-api-openapi.yml
  format: yaml
  label: Kurly 배송운영 정책 API
  slug: kurly-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-default-api-openapi.yml
- filename: kurly-delivery-tracking-api-openapi.yml
  format: yaml
  label: Kurly Delivery Tracking (배송추적) API
  slug: kurly-delivery-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-delivery-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kurly.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: kurly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kurly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kurly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kurly
provider_slug: kurly
slug: kurly-domain-security
source_filename: kurly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kurly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kurly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/security/kurly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Logistics
- Fulfillment
- Supply Chain
- Delivery
- Ecommerce
- Grocery
- Shipping
- Order Management
- Inventory
- Tracking
- South Korea
---
