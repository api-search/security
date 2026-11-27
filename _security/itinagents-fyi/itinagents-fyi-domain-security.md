---
api_specs:
- filename: itinagents-fyi-academy-api-openapi.yml
  format: yaml
  label: ITINAgents Academy API
  slug: itinagents-fyi-academy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-academy-api-openapi.yml
- filename: itinagents-fyi-admin-api-openapi.yml
  format: yaml
  label: ITINAgents Admin API
  slug: itinagents-fyi-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-admin-api-openapi.yml
- filename: itinagents-fyi-categories-api-openapi.yml
  format: yaml
  label: ITINAgents Categories API
  slug: itinagents-fyi-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-categories-api-openapi.yml
- filename: itinagents-fyi-certificates-api-openapi.yml
  format: yaml
  label: ITINAgents Certificates API
  slug: itinagents-fyi-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-certificates-api-openapi.yml
- filename: itinagents-fyi-listings-api-openapi.yml
  format: yaml
  label: ITINAgents Listings API
  slug: itinagents-fyi-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-listings-api-openapi.yml
- filename: itinagents-fyi-places-api-openapi.yml
  format: yaml
  label: ITINAgents Places API
  slug: itinagents-fyi-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-places-api-openapi.yml
- filename: itinagents-fyi-product-categories-api-openapi.yml
  format: yaml
  label: ITINAgents Product Categories API
  slug: itinagents-fyi-product-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-product-categories-api-openapi.yml
- filename: itinagents-fyi-products-api-openapi.yml
  format: yaml
  label: ITINAgents Products API
  slug: itinagents-fyi-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-products-api-openapi.yml
- filename: itinagents-fyi-sources-api-openapi.yml
  format: yaml
  label: ITINAgents Sources API
  slug: itinagents-fyi-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-sources-api-openapi.yml
- filename: itinagents-fyi-sponsor-api-openapi.yml
  format: yaml
  label: ITINAgents Sponsor API
  slug: itinagents-fyi-sponsor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-sponsor-api-openapi.yml
- filename: itinagents-fyi-stats-api-openapi.yml
  format: yaml
  label: ITINAgents Stats API
  slug: itinagents-fyi-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itinagents-fyi/openapi/itinagents-fyi-stats-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: itinagents.fyi
  spf: true
hosts:
- cert_expires: Jan 18 07:45:06 2027 GMT
  host: itinagents.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ITINAgents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ITINAgents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ITINAgents
provider_slug: itinagents-fyi
slug: itinagents-fyi-domain-security
source_filename: itinagents-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itinagents.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 07:45:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: itinagents.fyi\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/itinagents-fyi/security/itinagents-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Directory
- Tax
- IRS
- International
---
