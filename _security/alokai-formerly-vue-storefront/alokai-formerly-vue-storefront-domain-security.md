---
api_specs:
- filename: alokai-formerly-vue-storefront-cloud-openapi.json
  format: json
  label: Alokai Cloud API
  slug: alokai-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alokai-formerly-vue-storefront/refs/heads/main/openapi/alokai-formerly-vue-storefront-cloud-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alokai.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vuestorefront.cloud
  spf: false
hosts:
- cert_expires: Oct 10 06:40:30 2026 GMT
  host: alokai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 05:36:24 2026 GMT
  host: docs.alokai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 02:36:48 2026 GMT
  host: farmer.vuestorefront.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alokai Formerly Vue Storefront Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alokai (formerly Vue Storefront), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alokai (formerly Vue Storefront)
provider_slug: alokai-formerly-vue-storefront
slug: alokai-formerly-vue-storefront-domain-security
source_filename: alokai-formerly-vue-storefront-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alokai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:40:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.alokai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 05:36:24 2026 GMT\n  hsts: false\n- host: farmer.vuestorefront.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 02:36:48 2026 GMT\n  hsts: null\ndomains:\n- domain: alokai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vuestorefront.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alokai-formerly-vue-storefront/refs/heads/main/security/alokai-formerly-vue-storefront-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- Ecommerce
- Composable Commerce
- Headless Commerce
- Frontend as a Service
- Storefront
- SDK
- Middleware
- Cloud Hosting
---
