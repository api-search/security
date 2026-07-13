---
api_specs:
- filename: etsy-openapi-original.yml
  format: yaml
  label: Etsy Open API v3
  slug: open-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/openapi/etsy-openapi-original.yml
- filename: etsy-webhooks-asyncapi.yml
  format: yaml
  label: Etsy Open API v3 Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/asyncapi/etsy-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: etsy.com
  spf: true
hosts:
- cert_expires: Dec  5 15:09:44 2026 GMT
  host: www.etsy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 13:10:28 2026 GMT
  host: developers.etsy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 15:09:44 2026 GMT
  host: openapi.etsy.com
  hsts: true
  hsts_max_age: 631138520
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Etsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Etsy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Etsy
provider_slug: etsy
slug: etsy-domain-security
source_filename: etsy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.etsy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 15:09:44 2026 GMT\n  hsts: null\n- host: developers.etsy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 13:10:28 2026 GMT\n  hsts: false\n- host: openapi.etsy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 15:09:44 2026 GMT\n  hsts: true\n  hsts_max_age: 631138520\ndomains:\n- domain: etsy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/security/etsy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- Ecommerce
- Handmade
- Listings
- Orders
- Payments
- Reviews
- Shipping
- Taxonomy
- OAuth2
---
