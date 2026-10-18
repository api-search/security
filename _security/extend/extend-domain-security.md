---
api_specs:
- filename: extend-claims-management-api-openapi.yml
  format: yaml
  label: Extend Claims Management API
  slug: extend-claims-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-claims-management-api-openapi.yml
- filename: extend-contracts-api-openapi.yml
  format: yaml
  label: Extend Contracts API
  slug: extend-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-contracts-api-openapi.yml
- filename: extend-leads-api-openapi.yml
  format: yaml
  label: Extend Leads API
  slug: extend-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-leads-api-openapi.yml
- filename: extend-offers-api-openapi.yml
  format: yaml
  label: Extend Offers API
  slug: extend-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-offers-api-openapi.yml
- filename: extend-orders-api-openapi.yml
  format: yaml
  label: Extend Orders API
  slug: extend-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-orders-api-openapi.yml
- filename: extend-products-api-openapi.yml
  format: yaml
  label: Extend Products API
  slug: extend-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-products-api-openapi.yml
- filename: extend-refunds-api-openapi.yml
  format: yaml
  label: Extend Refunds API
  slug: extend-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-refunds-api-openapi.yml
- filename: extend-service-orders-api-openapi.yml
  format: yaml
  label: Extend Service Orders API
  slug: extend-service-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-service-orders-api-openapi.yml
- filename: extend-dynamic-return-policy-api-openapi.yml
  format: yaml
  label: Extend Dynamic Return Policy API
  slug: extend-dynamic-return-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-dynamic-return-policy-api-openapi.yml
- filename: extend-line-items-api-openapi.yml
  format: yaml
  label: Extend Line Items API
  slug: extend-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-line-items-api-openapi.yml
- filename: extend-shippingoffers-api-openapi.yml
  format: yaml
  label: Extend Shipping Offers API
  slug: extend-shippingoffers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-shippingoffers-api-openapi.yml
- filename: extend-webhooks-api-openapi.yml
  format: yaml
  label: Extend Webhooks API
  slug: extend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: extend.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: helloextend.com
  spf: true
hosts:
- cert_expires: Sep 20 08:47:51 2026 GMT
  host: docs.extend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.helloextend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Extend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extend, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Extend
provider_slug: extend
slug: extend-domain-security
source_filename: extend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.extend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:47:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.helloextend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: extend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: helloextend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/security/extend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Product Protection
- Extended Warranty
- Shipping Protection
- E-Commerce
- Warranty
- Claims
- Contracts
- Retail
- Insurance
---
