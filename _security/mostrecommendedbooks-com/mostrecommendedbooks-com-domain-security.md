---
api_specs:
- filename: mostrecommendedbooks-com-books-api-openapi.yml
  format: yaml
  label: Most Recommended Books Books API
  slug: mostrecommendedbooks-com-books-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mostrecommendedbooks-com/openapi/mostrecommendedbooks-com-books-api-openapi.yml
- filename: mostrecommendedbooks-com-lists-api-openapi.yml
  format: yaml
  label: Most Recommended Books Lists API
  slug: mostrecommendedbooks-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mostrecommendedbooks-com/openapi/mostrecommendedbooks-com-lists-api-openapi.yml
- filename: mostrecommendedbooks-com-people-api-openapi.yml
  format: yaml
  label: Most Recommended Books People API
  slug: mostrecommendedbooks-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mostrecommendedbooks-com/openapi/mostrecommendedbooks-com-people-api-openapi.yml
- filename: mostrecommendedbooks-com-series-api-openapi.yml
  format: yaml
  label: Most Recommended Books Series API
  slug: mostrecommendedbooks-com-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mostrecommendedbooks-com/openapi/mostrecommendedbooks-com-series-api-openapi.yml
- filename: mostrecommendedbooks-com-summaries-api-openapi.yml
  format: yaml
  label: Most Recommended Books Summaries API
  slug: mostrecommendedbooks-com-summaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mostrecommendedbooks-com/openapi/mostrecommendedbooks-com-summaries-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mostrecommendedbooks.com
  spf: false
hosts:
- cert_expires: Jan 19 19:05:56 2027 GMT
  host: mostrecommendedbooks.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Most Recommended Books Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Most Recommended Books, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Most Recommended Books
provider_slug: mostrecommendedbooks-com
slug: mostrecommendedbooks-com-domain-security
source_filename: mostrecommendedbooks-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mostrecommendedbooks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 19:05:56 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: mostrecommendedbooks.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mostrecommendedbooks-com/security/mostrecommendedbooks-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Book
- Recommendations
- Reading Lists
- Summary
- Literature
- Company
---
