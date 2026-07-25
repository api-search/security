---
api_specs:
- filename: news-api-articles-api-openapi.yml
  format: yaml
  label: News API Articles API
  slug: news-api-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-api/refs/heads/main/openapi/news-api-articles-api-openapi.yml
- filename: news-api-headlines-api-openapi.yml
  format: yaml
  label: News API Headlines API
  slug: news-api-headlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-api/refs/heads/main/openapi/news-api-headlines-api-openapi.yml
- filename: news-api-sources-api-openapi.yml
  format: yaml
  label: News API Sources API
  slug: news-api-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-api/refs/heads/main/openapi/news-api-sources-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: false
  dnssec: false
  domain: newsapi.org
  spf: true
hosts:
- cert_expires: Aug 15 23:59:59 2026 GMT
  host: newsapi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: News Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for News API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: News API
provider_slug: news-api
slug: news-api-domain-security
source_filename: news-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newsapi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: newsapi.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/news-api/refs/heads/main/security/news-api-domain-security.yml
summary_line: TLSv1.3
tags:
- News
- Articles
- Headlines
- Search
---
