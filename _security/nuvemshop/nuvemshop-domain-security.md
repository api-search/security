---
api_specs:
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Products API
  slug: nuvemshop-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Product Variants API
  slug: nuvemshop-product-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Product Images API
  slug: nuvemshop-product-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Categories API
  slug: nuvemshop-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Orders API
  slug: nuvemshop-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Customers API
  slug: nuvemshop-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Coupons API
  slug: nuvemshop-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Webhooks API
  slug: nuvemshop-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Scripts API
  slug: nuvemshop-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
- filename: nuvemshop-openapi.yml
  format: yaml
  label: Nuvemshop Store API
  slug: nuvemshop-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tiendanube.com
  spf: true
  spf_record: v=spf1 include:_spf.tiendanube_com._d.easydmarc.pro ~all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nuvemshop.com.br
  spf: true
  spf_record: v=spf1 include:_spf.nuvemshop_com_br._d.easydmarc.pro include:registrarmail.net ~all
hosts:
- cert_expires: Oct 10 08:15:08 2026 GMT
  host: api.tiendanube.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 07:31:38 2026 GMT
  host: tiendanube.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 06:31:23 2026 GMT
  host: www.tiendanube.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:55:29 2026 GMT
  host: nuvemshop.com.br
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuvemshop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuvemshop / Tiendanube, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nuvemshop / Tiendanube
provider_slug: nuvemshop
slug: nuvemshop-domain-security
source_filename: nuvemshop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.tiendanube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 08:15:08 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: tiendanube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:31:38 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: www.tiendanube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:31:23 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: nuvemshop.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:55:29 2026 GMT\n  hsts: false\n  hsts_max_age: null\ndomains:\n- domain: tiendanube.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.tiendanube_com._d.easydmarc.pro ~all'\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nuvemshop.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.nuvemshop_com_br._d.easydmarc.pro\
  \ include:registrarmail.net ~all'\n  dmarc: true\n  dmarc_policy: quarantine\nnotes: >-\n  All probed hosts serve HTTPS over TLS 1.3. No HTTP Strict-Transport-Security\n  (HSTS) response header was observed on the apex, www, or API hosts at probe\n  time. Neither apex domain publishes CAA records or has DNSSEC (DS) enabled.\n  Both domains publish SPF (soft-fail ~all) and DMARC at policy=quarantine\n  (pct=100), managed via EasyDMARC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/security/nuvemshop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-commerce
- Online Store
- Latin America
- Brazil
- Argentina
- Storefront
- Products
- Orders
- Merchants
- Webhooks
- SaaS
---
