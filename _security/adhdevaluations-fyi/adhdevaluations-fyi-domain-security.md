---
api_specs:
- filename: adhdevaluations-fyi-admin-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Admin API
  slug: adhdevaluations-fyi-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-admin-api-openapi.yml
- filename: adhdevaluations-fyi-categories-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Categories API
  slug: adhdevaluations-fyi-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-categories-api-openapi.yml
- filename: adhdevaluations-fyi-listings-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Listings API
  slug: adhdevaluations-fyi-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-listings-api-openapi.yml
- filename: adhdevaluations-fyi-places-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Places API
  slug: adhdevaluations-fyi-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-places-api-openapi.yml
- filename: adhdevaluations-fyi-sources-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Sources API
  slug: adhdevaluations-fyi-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-sources-api-openapi.yml
- filename: adhdevaluations-fyi-stats-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Stats API
  slug: adhdevaluations-fyi-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-stats-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adhdevaluations.fyi
  spf: true
hosts:
- cert_expires: Jan 18 07:57:36 2027 GMT
  host: adhdevaluations.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ADHDEvaluations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADHDEvaluations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ADHDEvaluations
provider_slug: adhdevaluations-fyi
slug: adhdevaluations-fyi-domain-security
source_filename: adhdevaluations-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adhdevaluations.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 07:57:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adhdevaluations.fyi\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/adhdevaluations-fyi/security/adhdevaluations-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ADHD
- Healthcare
- Directory
- Evaluation
- Providers
---
