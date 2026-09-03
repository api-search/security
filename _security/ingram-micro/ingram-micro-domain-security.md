---
api_specs:
- filename: ingram-micro-catalog-api-openapi.yml
  format: yaml
  label: ingram-micro Catalog API
  slug: ingram-micro-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/openapi/ingram-micro-catalog-api-openapi.yml
- filename: ingram-micro-inventory-api-openapi.yml
  format: yaml
  label: ingram-micro Inventory API
  slug: ingram-micro-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/openapi/ingram-micro-inventory-api-openapi.yml
- filename: ingram-micro-orders-api-openapi.yml
  format: yaml
  label: ingram-micro Orders API
  slug: ingram-micro-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/openapi/ingram-micro-orders-api-openapi.yml
- filename: ingram-micro-pricing-api-openapi.yml
  format: yaml
  label: ingram-micro Pricing API
  slug: ingram-micro-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/openapi/ingram-micro-pricing-api-openapi.yml
- filename: ingram-micro-shipments-api-openapi.yml
  format: yaml
  label: ingram-micro Shipments API
  slug: ingram-micro-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/openapi/ingram-micro-shipments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ingrammicro.com
  spf: true
hosts:
- cert_expires: Jul 16 23:59:59 2026 GMT
  host: developer.ingrammicro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.ingrammicro.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ingram Micro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ingram Micro, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ingram Micro
provider_slug: ingram-micro
slug: ingram-micro-domain-security
source_filename: ingram-micro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ingrammicro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.ingrammicro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ingrammicro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/security/ingram-micro-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Fortune 100
---
