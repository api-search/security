---
api_specs:
- filename: modivo-commerce-rest-api-openapi.yml
  format: yaml
  label: MODIVO Commerce REST API
  slug: modivo-commerce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modivo/refs/heads/main/openapi/modivo-commerce-rest-api-openapi.yml
- filename: modivo-eobuwie-commerce-rest-api-openapi.yml
  format: yaml
  label: eobuwie Commerce REST API
  slug: eobuwie-commerce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modivo/refs/heads/main/openapi/modivo-eobuwie-commerce-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modivo.pl
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eobuwie.com.pl
  spf: true
hosts:
- cert_expires: Sep 13 18:25:33 2026 GMT
  host: modivo.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 01:06:51 2026 GMT
  host: eobuwie.com.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 04:04:14 2026 GMT
  host: modivo.mirakl.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modivo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MODIVO, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MODIVO
provider_slug: modivo
slug: modivo-domain-security
source_filename: modivo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modivo.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:25:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eobuwie.com.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 01:06:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: modivo.mirakl.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 04:04:14 2026 GMT\n  hsts: null\ndomains:\n- domain: modivo.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: eobuwie.com.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modivo/refs/heads/main/security/modivo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fashion
- E-Commerce
- Retail
- Marketplace
- Retail Media
- Commerce
- Checkout
- Catalog
- GraphQL
- Adobe Commerce
- Magento
- Poland
- Central Europe
---
