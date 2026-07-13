---
api_specs:
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Ingredients API
  slug: ingredients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Recipes API
  slug: recipes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Products API
  slug: products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Inventory & Stock API
  slug: inventory-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Purchase Orders API
  slug: purchase-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Suppliers API
  slug: suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Outlets API
  slug: outlets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "rapidssl.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: apicbase.com
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.apicbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  4 01:02:15 2026 GMT
  host: developers.apicbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: api.apicbase.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Apicbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apicbase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Apicbase
provider_slug: apicbase
slug: apicbase-domain-security
source_filename: apicbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apicbase.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.apicbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:02:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apicbase.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: apicbase.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/security/apicbase-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Food and Beverage
- Restaurant
- Back of House
- Inventory
- Procurement
- Recipes
---
