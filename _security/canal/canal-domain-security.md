---
api_specs:
- filename: canal-openapi-original.yml
  format: yaml
  label: Rokt Catalog Platform API
  slug: rokt-catalog-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shopcanal.com
  spf: true
hosts:
- cert_expires: Aug 23 02:46:25 2026 GMT
  host: api.shopcanal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Canal
provider_slug: canal
slug: canal-domain-security
source_filename: canal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.shopcanal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 02:46:25 2026 GMT\n  hsts: false\ndomains:\n- domain: shopcanal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/security/canal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- eCommerce
- Dropshipping
- Marketplace
- Commerce
- Retail
- Fulfillment
- Orders
- Products
- Webhooks
---
