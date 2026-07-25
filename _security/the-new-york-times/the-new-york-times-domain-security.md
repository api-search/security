---
api_specs:
- filename: the-new-york-times-archive-api-openapi.yml
  format: yaml
  label: The New York Times Archive API
  slug: the-new-york-times-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-archive-api-openapi.yml
- filename: the-new-york-times-content-api-openapi.yml
  format: yaml
  label: The New York Times Content API
  slug: the-new-york-times-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-content-api-openapi.yml
- filename: the-new-york-times-movies-api-openapi.yml
  format: yaml
  label: The New York Times Movies API
  slug: the-new-york-times-movies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-movies-api-openapi.yml
- filename: the-new-york-times-name-api-openapi.yml
  format: yaml
  label: The New York Times Name API
  slug: the-new-york-times-name-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-name-api-openapi.yml
- filename: the-new-york-times-search-api-openapi.yml
  format: yaml
  label: The New York Times Search API
  slug: the-new-york-times-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-search-api-openapi.yml
- filename: the-new-york-times-stories-api-openapi.yml
  format: yaml
  label: The New York Times Stories API
  slug: the-new-york-times-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-stories-api-openapi.yml
- filename: the-new-york-times-timestags-api-openapi.yml
  format: yaml
  label: The New York Times Timestags API
  slug: the-new-york-times-timestags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-timestags-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
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
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: nytimes.com
  hsts: true
  hsts_max_age: 63072000
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
name: The New York Times Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The New York Times, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The New York Times
provider_slug: the-new-york-times
slug: the-new-york-times-domain-security
source_filename: the-new-york-times-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.nytimes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 03:39:39 2026 GMT\n  hsts: null\n- host: nytimes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nytimes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:39:28 2026 GMT\n  hsts: null\ndomains:\n- domain: nytimes.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/security/the-new-york-times-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Articles
- Books
- Movies
- News
- Media
- Publishing
- Journalism
---
