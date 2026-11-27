---
api_specs:
- filename: opioidtreatment-fyi-academy-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Academy API
  slug: opioidtreatment-fyi-academy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-academy-api-openapi.yml
- filename: opioidtreatment-fyi-admin-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Admin API
  slug: opioidtreatment-fyi-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-admin-api-openapi.yml
- filename: opioidtreatment-fyi-categories-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Categories API
  slug: opioidtreatment-fyi-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-categories-api-openapi.yml
- filename: opioidtreatment-fyi-certificates-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Certificates API
  slug: opioidtreatment-fyi-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-certificates-api-openapi.yml
- filename: opioidtreatment-fyi-listings-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Listings API
  slug: opioidtreatment-fyi-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-listings-api-openapi.yml
- filename: opioidtreatment-fyi-places-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Places API
  slug: opioidtreatment-fyi-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-places-api-openapi.yml
- filename: opioidtreatment-fyi-product-categories-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Product Categories API
  slug: opioidtreatment-fyi-product-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-product-categories-api-openapi.yml
- filename: opioidtreatment-fyi-products-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Products API
  slug: opioidtreatment-fyi-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-products-api-openapi.yml
- filename: opioidtreatment-fyi-sources-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Sources API
  slug: opioidtreatment-fyi-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-sources-api-openapi.yml
- filename: opioidtreatment-fyi-sponsor-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Sponsor API
  slug: opioidtreatment-fyi-sponsor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-sponsor-api-openapi.yml
- filename: opioidtreatment-fyi-stats-api-openapi.yml
  format: yaml
  label: Opioid Treatment Directory Stats API
  slug: opioidtreatment-fyi-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opioidtreatment-fyi/openapi/opioidtreatment-fyi-stats-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opioidtreatment.fyi
  spf: true
hosts:
- cert_expires: Jan 18 07:36:41 2027 GMT
  host: opioidtreatment.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opioid Treatment Directory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opioid Treatment Directory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Opioid Treatment Directory
provider_slug: opioidtreatment-fyi
slug: opioidtreatment-fyi-domain-security
source_filename: opioidtreatment-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opioidtreatment.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 07:36:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: opioidtreatment.fyi\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/opioidtreatment-fyi/security/opioidtreatment-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Directory
- OpioidTreatment
---
