---
api_specs:
- filename: article-search-v2-openapi.yml
  format: yaml
  label: Article Search API
  slug: article-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/article-search-v2-openapi.yml
- filename: top-stories-v2-openapi.yml
  format: yaml
  label: Top Stories API
  slug: top-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/top-stories-v2-openapi.yml
- filename: most-popular-api-v2-openapi.yml
  format: yaml
  label: Most Popular API
  slug: most-popular-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/most-popular-api-v2-openapi.yml
- filename: timeswire-v3-openapi.yml
  format: yaml
  label: Times Newswire API
  slug: times-newswire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/timeswire-v3-openapi.yml
- filename: archive-api-openapi.yml
  format: yaml
  label: Archive API
  slug: archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/archive-api-openapi.yml
- filename: books-api-openapi.yml
  format: yaml
  label: Books API
  slug: books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/books-api-openapi.yml
- filename: movie-reviews-v2-openapi.yml
  format: yaml
  label: Movie Reviews API
  slug: movie-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/movie-reviews-v2-openapi.yml
- filename: times-tags-v3-openapi.yml
  format: yaml
  label: TimesTags API
  slug: timestags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/times-tags-v3-openapi.yml
- filename: semantic-api-openapi.yml
  format: yaml
  label: Semantic API
  slug: semantic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/semantic-api-openapi.yml
- filename: geo-api-v2-openapi.yml
  format: yaml
  label: Geographic API
  slug: geographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/geo-api-v2-openapi.yml
- filename: community-api-v3-openapi.yml
  format: yaml
  label: Community API (Deprecated)
  slug: community-api-deprecated
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/community-api-v3-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nytimes.com
  spf: true
hosts:
- cert_expires: Aug 20 03:39:39 2026 GMT
  host: developer.nytimes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 11:39:28 2026 GMT
  host: api.nytimes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: New York Times Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The New York Times Company, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The New York Times Company
provider_slug: new-york-times-company
slug: new-york-times-company-domain-security
source_filename: new-york-times-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.nytimes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 03:39:39 2026 GMT\n  hsts: null\n- host: api.nytimes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:39:28 2026 GMT\n  hsts: null\ndomains:\n- domain: nytimes.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/security/new-york-times-company-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Media
- Publishing
- Newspapers
- Articles
- Books
- Movies
- Sports
- Games
- Cooking
- Reviews
- Search
- Semantic
- Tagging
- Controlled Vocabulary
- Geographic
- Archive
---
