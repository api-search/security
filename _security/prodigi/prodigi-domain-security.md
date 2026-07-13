---
api_specs:
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Orders API
  slug: prodigi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Quotes API
  slug: prodigi-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Product Details API
  slug: prodigi-product-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Webhooks / Callbacks
  slug: prodigi-webhooks-callbacks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prodigi.com
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.prodigi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.prodigi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.sandbox.prodigi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prodigi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prodigi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prodigi
provider_slug: prodigi
slug: prodigi-domain-security
source_filename: prodigi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prodigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.prodigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\n- host: api.sandbox.prodigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: prodigi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/security/prodigi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Print on Demand
- Printing
- Dropshipping
- Fulfillment
- E-commerce
---
