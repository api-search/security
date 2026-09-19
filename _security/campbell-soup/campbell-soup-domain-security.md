---
api_specs:
- filename: campbell-soup-authors-api-openapi.yml
  format: yaml
  label: Campbell Soup Authors API
  slug: campbell-soup-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-authors-api-openapi.yml
- filename: campbell-soup-comments-api-openapi.yml
  format: yaml
  label: Campbell Soup Comments API
  slug: campbell-soup-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-comments-api-openapi.yml
- filename: campbell-soup-discovery-api-openapi.yml
  format: yaml
  label: Campbell Soup Discovery API
  slug: campbell-soup-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-discovery-api-openapi.yml
- filename: campbell-soup-external-products-api-openapi.yml
  format: yaml
  label: Campbell Soup External Products API
  slug: campbell-soup-external-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-external-products-api-openapi.yml
- filename: campbell-soup-media-api-openapi.yml
  format: yaml
  label: Campbell Soup Media API
  slug: campbell-soup-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-media-api-openapi.yml
- filename: campbell-soup-pages-api-openapi.yml
  format: yaml
  label: Campbell Soup Pages API
  slug: campbell-soup-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-pages-api-openapi.yml
- filename: campbell-soup-posts-api-openapi.yml
  format: yaml
  label: Campbell Soup Posts API
  slug: campbell-soup-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-posts-api-openapi.yml
- filename: campbell-soup-products-api-openapi.yml
  format: yaml
  label: Campbell Soup Products API
  slug: campbell-soup-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-products-api-openapi.yml
- filename: campbell-soup-recipes-api-openapi.yml
  format: yaml
  label: Campbell Soup Recipes API
  slug: campbell-soup-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-recipes-api-openapi.yml
- filename: campbell-soup-search-api-openapi.yml
  format: yaml
  label: Campbell Soup Search API
  slug: campbell-soup-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-search-api-openapi.yml
- filename: campbell-soup-taxonomies-api-openapi.yml
  format: yaml
  label: Campbell Soup Taxonomies API
  slug: campbell-soup-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-taxonomies-api-openapi.yml
- filename: campbell-soup-faqs-api-openapi.yml
  format: yaml
  label: Campbell Soup FA Qs API
  slug: campbell-soup-faqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/openapi/campbell-soup-faqs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thecampbellscompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: campbellskitchen.com
  spf: true
hosts:
- cert_expires: Nov 29 02:04:50 2026 GMT
  host: www.thecampbellscompany.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.campbellskitchen.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Campbell Soup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campbell Soup, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Campbell Soup
provider_slug: campbell-soup
slug: campbell-soup-domain-security
source_filename: campbell-soup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thecampbellscompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 02:04:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.campbellskitchen.com\n  https: false\ndomains:\n- domain: thecampbellscompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: campbellskitchen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/security/campbell-soup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food
- Consumer Packaged Goods
- Recipes
- Product
- Nutrition
- Brands
- Fortune 500
- content-api
- WordPress
---
