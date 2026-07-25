---
api_specs:
- filename: google-news-headlines-api-openapi.yml
  format: yaml
  label: Google News RSS Headlines API
  slug: google-news-headlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-news/refs/heads/main/openapi/google-news-headlines-api-openapi.yml
- filename: google-news-search-api-openapi.yml
  format: yaml
  label: Google News RSS Search API
  slug: google-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-news/refs/heads/main/openapi/google-news-search-api-openapi.yml
- filename: google-news-topics-api-openapi.yml
  format: yaml
  label: Google News RSS Topics API
  slug: google-news-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-news/refs/heads/main/openapi/google-news-topics-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Sep 14 08:37:53 2026 GMT
  host: news.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google News Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google News RSS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google News RSS
provider_slug: google-news
slug: google-news-domain-security
source_filename: google-news-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: news.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-news/refs/heads/main/security/google-news-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aggregation
- Google News
- Headlines
- Media
- News
- RSS
---
