---
api_specs:
- filename: noozra-building-permits-api-openapi.yml
  format: yaml
  label: Noozra Building permits API
  slug: noozra-building-permits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-building-permits-api-openapi.yml
- filename: noozra-communities-api-openapi.yml
  format: yaml
  label: Noozra Communities API
  slug: noozra-communities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-communities-api-openapi.yml
- filename: noozra-datasets-api-openapi.yml
  format: yaml
  label: Noozra Datasets API
  slug: noozra-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-datasets-api-openapi.yml
- filename: noozra-federal-register-api-openapi.yml
  format: yaml
  label: Noozra Federal Register API
  slug: noozra-federal-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-federal-register-api-openapi.yml
- filename: noozra-government-contracts-api-openapi.yml
  format: yaml
  label: Noozra Government contracts API
  slug: noozra-government-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-government-contracts-api-openapi.yml
- filename: noozra-jobs-api-openapi.yml
  format: yaml
  label: Noozra Jobs API
  slug: noozra-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-jobs-api-openapi.yml
- filename: noozra-new-businesses-api-openapi.yml
  format: yaml
  label: Noozra New businesses API
  slug: noozra-new-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-new-businesses-api-openapi.yml
- filename: noozra-news-api-openapi.yml
  format: yaml
  label: Noozra News API
  slug: noozra-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-news-api-openapi.yml
- filename: noozra-product-recalls-api-openapi.yml
  format: yaml
  label: Noozra Product recalls API
  slug: noozra-product-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-product-recalls-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: noozra.com
  spf: true
hosts:
- cert_expires: Jan 28 01:42:32 2027 GMT
  host: noozra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Noozra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noozra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Noozra
provider_slug: noozra
slug: noozra-domain-security
source_filename: noozra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noozra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 01:42:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noozra.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/noozra/security/noozra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- News
- Free
- Community
- Artificial Intelligence
---
