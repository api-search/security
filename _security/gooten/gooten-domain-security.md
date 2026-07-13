---
api_specs:
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Products API
  slug: gooten-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Orders API
  slug: gooten-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Shipping API
  slug: gooten-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Print Assets API
  slug: gooten-print-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gooten.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: print.io
  spf: true
hosts:
- cert_expires: Aug 28 23:59:59 2026 GMT
  host: www.gooten.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.print.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gooten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gooten, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gooten
provider_slug: gooten
slug: gooten-domain-security
source_filename: gooten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gooten.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.print.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gooten.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: print.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/security/gooten-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Print on Demand
- Fulfillment
- Manufacturing
- Ecommerce
- Dropshipping
- Custom Products
---
