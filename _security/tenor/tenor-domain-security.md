---
api_specs:
- filename: tenor-autocomplete-api-openapi.yml
  format: yaml
  label: Tenor Autocomplete API
  slug: tenor-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-autocomplete-api-openapi.yml
- filename: tenor-categories-api-openapi.yml
  format: yaml
  label: Tenor Categories API
  slug: tenor-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-categories-api-openapi.yml
- filename: tenor-featured-api-openapi.yml
  format: yaml
  label: Tenor Featured API
  slug: tenor-featured-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-featured-api-openapi.yml
- filename: tenor-posts-api-openapi.yml
  format: yaml
  label: Tenor Posts API
  slug: tenor-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-posts-api-openapi.yml
- filename: tenor-registershare-api-openapi.yml
  format: yaml
  label: Tenor Registershare API
  slug: tenor-registershare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-registershare-api-openapi.yml
- filename: tenor-search-api-openapi.yml
  format: yaml
  label: Tenor Search API
  slug: tenor-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-search-api-openapi.yml
- filename: tenor-search-suggestions-api-openapi.yml
  format: yaml
  label: Tenor Search Suggestions API
  slug: tenor-search-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-search-suggestions-api-openapi.yml
- filename: tenor-trending-terms-api-openapi.yml
  format: yaml
  label: Tenor Trending Terms API
  slug: tenor-trending-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-trending-terms-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tenor.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Jan 25 17:32:49 2027 GMT
  host: tenor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: tenor.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Tenor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tenor
provider_slug: tenor
slug: tenor-domain-security
source_filename: tenor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tenor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 17:32:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tenor.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: tenor.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tenor/security/tenor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GIFs
- Animated Images
- Search
- Media
- Google
---
