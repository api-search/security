---
api_specs:
- filename: cresilon-posts-api-openapi.yml
  format: yaml
  label: Cresilon News & Press Releases API
  slug: cresilon-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-posts-api-openapi.yml
- filename: cresilon-pages-api-openapi.yml
  format: yaml
  label: Cresilon Pages API
  slug: cresilon-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-pages-api-openapi.yml
- filename: cresilon-media-api-openapi.yml
  format: yaml
  label: Cresilon Media API
  slug: cresilon-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-media-api-openapi.yml
- filename: cresilon-taxonomy-api-openapi.yml
  format: yaml
  label: Cresilon Taxonomy API
  slug: cresilon-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-taxonomy-api-openapi.yml
- filename: cresilon-search-api-openapi.yml
  format: yaml
  label: Cresilon Search API
  slug: cresilon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-search-api-openapi.yml
- filename: cresilon-discovery-api-openapi.yml
  format: yaml
  label: Cresilon Discovery API
  slug: cresilon-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-discovery-api-openapi.yml
- filename: cresilon-oembed-api-openapi.yml
  format: yaml
  label: Cresilon oEmbed API
  slug: cresilon-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-oembed-api-openapi.yml
- filename: cresilon-seo-api-openapi.yml
  format: yaml
  label: Cresilon SEO Metadata API
  slug: cresilon-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-seo-api-openapi.yml
- filename: cresilon-authors-api-openapi.yml
  format: yaml
  label: Cresilon Authors API
  slug: cresilon-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-authors-api-openapi.yml
- filename: cresilon-comments-api-openapi.yml
  format: yaml
  label: Cresilon Comments API
  slug: cresilon-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-comments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cresilon.com
  spf: true
hosts:
- api_host: true
  api_note: cresilon.com is also the API host — the WordPress REST surface is served from the same origin at /wp-json/. No api./developer./docs./status./trust. subdomain exists (all failed to resolve), so there is no second host to probe.
  cert_expires: Nov  2 09:01:27 2026 GMT
  host: cresilon.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  note: 'HSTS was re-probed by hand on 2026-08-04 and IS present — `strict-transport-security: max-age=31536000` is returned on both https://cresilon.com/ and the wp-json API routes. The automated pass recorded null; the observed header value above supersedes it.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cresilon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cresilon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cresilon
provider_slug: cresilon
slug: cresilon-domain-security
source_filename: cresilon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cresilon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 09:01:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  hsts_preload: false\n  note: >-\n    HSTS was re-probed by hand on 2026-08-04 and IS present — `strict-transport-security:\n    max-age=31536000` is returned on both https://cresilon.com/ and the wp-json API routes. The\n    automated pass recorded null; the observed header value above supersedes it.\n  api_host: true\n  api_note: >-\n    cresilon.com is also the API host — the WordPress REST surface is served from the same origin\n    at /wp-json/. No api./developer./docs./status./trust. subdomain exists (all failed to\n    resolve), so there is no second host to probe.\ndomains:\n- domain: cresilon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/security/cresilon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Medical Devices
- Health
- Hemostasis
- Wound Care
- Trauma Care
- Veterinary
- Life Sciences
- Manufacturing
- Content
---
