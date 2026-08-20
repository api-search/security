---
api_specs:
- filename: duda-accounts-api-openapi.yml
  format: yaml
  label: Duda Accounts API
  slug: duda-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-accounts-api-openapi.yml
- filename: duda-authentication-api-openapi.yml
  format: yaml
  label: Duda Authentication API
  slug: duda-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-authentication-api-openapi.yml
- filename: duda-blog-api-openapi.yml
  format: yaml
  label: Duda Blog API
  slug: duda-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-blog-api-openapi.yml
- filename: duda-collections-api-openapi.yml
  format: yaml
  label: Duda Collections API
  slug: duda-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-collections-api-openapi.yml
- filename: duda-ecommerce-orders-api-openapi.yml
  format: yaml
  label: Duda eCommerce - Orders API
  slug: duda-ecommerce-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-ecommerce-orders-api-openapi.yml
- filename: duda-ecommerce-products-api-openapi.yml
  format: yaml
  label: Duda eCommerce - Products API
  slug: duda-ecommerce-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-ecommerce-products-api-openapi.yml
- filename: duda-pages-api-openapi.yml
  format: yaml
  label: Duda Pages API
  slug: duda-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-pages-api-openapi.yml
- filename: duda-sites-api-openapi.yml
  format: yaml
  label: Duda Sites API
  slug: duda-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-sites-api-openapi.yml
- filename: duda-templates-api-openapi.yml
  format: yaml
  label: Duda Templates API
  slug: duda-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-templates-api-openapi.yml
- filename: duda-webhooks-api-openapi.yml
  format: yaml
  label: Duda Webhooks API
  slug: duda-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: duda.co
  spf: true
hosts:
- cert_expires: Sep 18 03:42:05 2026 GMT
  host: www.duda.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 14:30:47 2026 GMT
  host: developer.duda.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.duda.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duda, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Duda
provider_slug: duda
slug: duda-domain-security
source_filename: duda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.duda.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:42:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.duda.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:30:47 2026 GMT\n  hsts: null\n- host: api.duda.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: duda.co\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/security/duda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Website Builder
- Agencies
- White Label
- Software-as-a-Service
- E-Commerce
- CMS
---
