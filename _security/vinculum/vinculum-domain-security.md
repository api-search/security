---
api_specs:
- filename: vinculum-advance-shipping-notice-api-openapi.yml
  format: yaml
  label: Vinculum Advance Shipping Notice API
  slug: vinculum-advance-shipping-notice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-advance-shipping-notice-api-openapi.yml
- filename: vinculum-authentication-process-api-openapi.yml
  format: yaml
  label: Vinculum Authentication Process API
  slug: vinculum-authentication-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-authentication-process-api-openapi.yml
- filename: vinculum-common-api-openapi.yml
  format: yaml
  label: Vinculum Common API
  slug: vinculum-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-common-api-openapi.yml
- filename: vinculum-courier-allocation-process-api-openapi.yml
  format: yaml
  label: Vinculum Courier Allocation Process API
  slug: vinculum-courier-allocation-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-courier-allocation-process-api-openapi.yml
- filename: vinculum-inbounds-api-openapi.yml
  format: yaml
  label: Vinculum Inbounds API
  slug: vinculum-inbounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-inbounds-api-openapi.yml
- filename: vinculum-listing-managment-api-openapi.yml
  format: yaml
  label: Vinculum Listing Managment API
  slug: vinculum-listing-managment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-listing-managment-api-openapi.yml
- filename: vinculum-manifest-api-openapi.yml
  format: yaml
  label: Vinculum Manifest API
  slug: vinculum-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-manifest-api-openapi.yml
- filename: vinculum-order-managment-api-openapi.yml
  format: yaml
  label: Vinculum Order Managment API
  slug: vinculum-order-managment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-order-managment-api-openapi.yml
- filename: vinculum-order-returns-api-openapi.yml
  format: yaml
  label: Vinculum Order Returns API
  slug: vinculum-order-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-order-returns-api-openapi.yml
- filename: vinculum-orders-api-openapi.yml
  format: yaml
  label: Vinculum Orders API
  slug: vinculum-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-orders-api-openapi.yml
- filename: vinculum-products-api-openapi.yml
  format: yaml
  label: Vinculum Products API
  slug: vinculum-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-products-api-openapi.yml
- filename: vinculum-purchase-orders-api-openapi.yml
  format: yaml
  label: Vinculum Purchase Orders API
  slug: vinculum-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-purchase-orders-api-openapi.yml
- filename: vinculum-putaway-api-openapi.yml
  format: yaml
  label: Vinculum Putaway API
  slug: vinculum-putaway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-putaway-api-openapi.yml
- filename: vinculum-return-to-vendor-api-openapi.yml
  format: yaml
  label: Vinculum Return to Vendor API
  slug: vinculum-return-to-vendor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-return-to-vendor-api-openapi.yml
- filename: vinculum-stock-api-openapi.yml
  format: yaml
  label: Vinculum Stock API
  slug: vinculum-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-stock-api-openapi.yml
- filename: vinculum-transfers-api-openapi.yml
  format: yaml
  label: Vinculum Transfers API
  slug: vinculum-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-transfers-api-openapi.yml
- filename: vinculum-vendors-api-openapi.yml
  format: yaml
  label: Vinculum Vendors API
  slug: vinculum-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-vendors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vinculumgroup.com
  spf: true
hosts:
- cert_expires: Sep  7 18:48:52 2026 GMT
  host: www.vinculumgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vinculum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vinculum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vinculum
provider_slug: vinculum
slug: vinculum-domain-security
source_filename: vinculum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vinculumgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 18:48:52 2026 GMT\n  hsts: null\ndomains:\n- domain: vinculumgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/security/vinculum-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- E-Commerce
- Omnichannel
- Order Management
- Warehouse Management
- Inventory
- Retail
- Marketplaces
---
