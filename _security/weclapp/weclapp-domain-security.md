---
api_specs:
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Customer API
  slug: weclapp-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Article API
  slug: weclapp-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Sales Order API
  slug: weclapp-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Quotation API
  slug: weclapp-quotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Sales Invoice API
  slug: weclapp-sales-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Shipment API
  slug: weclapp-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Purchase Order API
  slug: weclapp-purchase-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: weclapp.com
  spf: true
  spf_policy: -all
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: weclapp.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  hsts_preload: true
  https: true
  note: Redirects to https://www.weclapp.com/. Served by nginx.
  tls_version: TLSv1.3
- host: www.weclapp.com
  hsts: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weclapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for weclapp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: weclapp
provider_slug: weclapp
slug: weclapp-domain-security
source_filename: weclapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (per-tenant API host not probeable without a real tenant)\nhosts:\n- host: weclapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Redirects to https://www.weclapp.com/. Served by nginx.\n- host: www.weclapp.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\ndomains:\n- domain: weclapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  dmarc: true\n  dmarc_policy: none\nnotes: >-\n  The REST API is served per tenant at https://<tenant>.weclapp.com/webapp/api/v1/.\n  There is no shared, tenant-agnostic API host to probe, so TLS/HSTS results above\n  are for the corporate/apex domain (weclapp.com) and its www host. Tenant hosts\n  inherit the weclapp.com wildcard TLS and HSTS includeSubDomains/preload policy.\nmaintainers:\n\
  - FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/security/weclapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ERP
- CRM
- Cloud ERP
- Accounting
- Inventory
- Commerce
- Germany
- Order Management
- Business Software
- SaaS
---
