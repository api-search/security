---
api_specs:
- filename: lish-categories-api-openapi.yml
  format: yaml
  label: Lish Categories API
  slug: lish-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-categories-api-openapi.yml
- filename: lish-comments-api-openapi.yml
  format: yaml
  label: Lish Comments API
  slug: lish-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-comments-api-openapi.yml
- filename: lish-media-api-openapi.yml
  format: yaml
  label: Lish Media API
  slug: lish-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-media-api-openapi.yml
- filename: lish-pages-api-openapi.yml
  format: yaml
  label: Lish Pages API
  slug: lish-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-pages-api-openapi.yml
- filename: lish-posts-api-openapi.yml
  format: yaml
  label: Lish Posts API
  slug: lish-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-posts-api-openapi.yml
- filename: lish-search-api-openapi.yml
  format: yaml
  label: Lish Search API
  slug: lish-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-search-api-openapi.yml
- filename: lish-statuses-api-openapi.yml
  format: yaml
  label: Lish Statuses API
  slug: lish-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-statuses-api-openapi.yml
- filename: lish-tags-api-openapi.yml
  format: yaml
  label: Lish Tags API
  slug: lish-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-tags-api-openapi.yml
- filename: lish-taxonomies-api-openapi.yml
  format: yaml
  label: Lish Taxonomies API
  slug: lish-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-taxonomies-api-openapi.yml
- filename: lish-types-api-openapi.yml
  format: yaml
  label: Lish Types API
  slug: lish-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-types-api-openapi.yml
- filename: lish-users-api-openapi.yml
  format: yaml
  label: Lish Users API
  slug: lish-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/openapi/lish-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lishfood.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: lishfood.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.lishfood.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lish, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lish
provider_slug: lish
slug: lish-domain-security
source_filename: lish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lishfood.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.lishfood.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lishfood.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lish/refs/heads/main/security/lish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Catering
- Food and Beverage
- Food Delivery
- Workplace
- Corporate Services
- Content
---
