---
api_specs:
- filename: leapcure-categories-api-openapi.yml
  format: yaml
  label: Leapcure categories API
  slug: leapcure-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-categories-api-openapi.yml
- filename: leapcure-comments-api-openapi.yml
  format: yaml
  label: Leapcure comments API
  slug: leapcure-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-comments-api-openapi.yml
- filename: leapcure-media-api-openapi.yml
  format: yaml
  label: Leapcure media API
  slug: leapcure-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-media-api-openapi.yml
- filename: leapcure-pages-api-openapi.yml
  format: yaml
  label: Leapcure pages API
  slug: leapcure-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-pages-api-openapi.yml
- filename: leapcure-posts-api-openapi.yml
  format: yaml
  label: Leapcure posts API
  slug: leapcure-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-posts-api-openapi.yml
- filename: leapcure-search-api-openapi.yml
  format: yaml
  label: Leapcure search API
  slug: leapcure-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-search-api-openapi.yml
- filename: leapcure-statuses-api-openapi.yml
  format: yaml
  label: Leapcure statuses API
  slug: leapcure-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-statuses-api-openapi.yml
- filename: leapcure-tags-api-openapi.yml
  format: yaml
  label: Leapcure tags API
  slug: leapcure-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-tags-api-openapi.yml
- filename: leapcure-taxonomies-api-openapi.yml
  format: yaml
  label: Leapcure taxonomies API
  slug: leapcure-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-taxonomies-api-openapi.yml
- filename: leapcure-types-api-openapi.yml
  format: yaml
  label: Leapcure types API
  slug: leapcure-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-types-api-openapi.yml
- filename: leapcure-users-api-openapi.yml
  format: yaml
  label: Leapcure users API
  slug: leapcure-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leapcure.com
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: leapcure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leapcure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leapcure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Leapcure
provider_slug: leapcure
slug: leapcure-domain-security
source_filename: leapcure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leapcure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leapcure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/security/leapcure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Clinical Trials
- Patient Recruitment
- Healthcare
- Blog
- content-api
- WordPress
---
