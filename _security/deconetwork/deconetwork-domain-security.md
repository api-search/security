---
api_specs:
- filename: deconetwork-inventory-api-openapi.yml
  format: yaml
  label: DecoNetwork Inventory API
  slug: deconetwork-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/openapi/deconetwork-inventory-api-openapi.yml
- filename: deconetwork-orders-api-openapi.yml
  format: yaml
  label: DecoNetwork Orders API
  slug: deconetwork-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/openapi/deconetwork-orders-api-openapi.yml
- filename: deconetwork-products-api-openapi.yml
  format: yaml
  label: DecoNetwork Products API
  slug: deconetwork-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/openapi/deconetwork-products-api-openapi.yml
- filename: deconetwork-purchase-orders-api-openapi.yml
  format: yaml
  label: DecoNetwork Purchase Orders API
  slug: deconetwork-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/openapi/deconetwork-purchase-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deconetwork.com
  spf: true
hosts:
- cert_expires: Aug 11 08:41:42 2026 GMT
  host: www.deconetwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:50:28 2026 GMT
  host: developer.deconetwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deconetwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DecoNetwork, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DecoNetwork
provider_slug: deconetwork
slug: deconetwork-domain-security
source_filename: deconetwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deconetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 08:41:42 2026 GMT\n  hsts: null\n- host: developer.deconetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:50:28 2026 GMT\n  hsts: false\ndomains:\n- domain: deconetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deconetwork/refs/heads/main/security/deconetwork-domain-security.yml
summary_line: TLSv1.3
tags:
- Custom Apparel
- Web to Print
- Print Shop Management
- Order
- Product
- Inventory
- Production Workflow
- E-Commerce
---
