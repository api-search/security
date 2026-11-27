---
api_specs:
- filename: opencapital-sh-business-profiles-api-openapi.yml
  format: yaml
  label: OpenCapital Business profiles API
  slug: opencapital-sh-business-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-business-profiles-api-openapi.yml
- filename: opencapital-sh-companies-api-openapi.yml
  format: yaml
  label: OpenCapital Companies API
  slug: opencapital-sh-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-companies-api-openapi.yml
- filename: opencapital-sh-filings-api-openapi.yml
  format: yaml
  label: OpenCapital Filings API
  slug: opencapital-sh-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-filings-api-openapi.yml
- filename: opencapital-sh-metrics-and-segments-api-openapi.yml
  format: yaml
  label: OpenCapital Metrics and segments API
  slug: opencapital-sh-metrics-and-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-metrics-and-segments-api-openapi.yml
- filename: opencapital-sh-reported-earnings-api-openapi.yml
  format: yaml
  label: OpenCapital Reported earnings API
  slug: opencapital-sh-reported-earnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-reported-earnings-api-openapi.yml
- filename: opencapital-sh-screening-api-openapi.yml
  format: yaml
  label: OpenCapital Screening API
  slug: opencapital-sh-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opencapital-sh/openapi/opencapital-sh-screening-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: opencapital.sh
  spf: false
hosts:
- cert_expires: Dec 27 15:15:59 2026 GMT
  host: opencapital.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenCapital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCapital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenCapital
provider_slug: opencapital-sh
slug: opencapital-sh-domain-security
source_filename: opencapital-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencapital.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 15:15:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opencapital.sh\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/opencapital-sh/security/opencapital-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- SEC Filings
- Financial Data
- Earnings
- Company screener
---
