---
api_specs:
- filename: beyourcover-com-account-api-openapi.yml
  format: yaml
  label: BeYourCover Account API
  slug: beyourcover-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-account-api-openapi.yml
- filename: beyourcover-com-books-api-openapi.yml
  format: yaml
  label: BeYourCover Books API
  slug: beyourcover-com-books-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-books-api-openapi.yml
- filename: beyourcover-com-clients-api-openapi.yml
  format: yaml
  label: BeYourCover Clients API
  slug: beyourcover-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-clients-api-openapi.yml
- filename: beyourcover-com-covers-api-openapi.yml
  format: yaml
  label: BeYourCover Covers API
  slug: beyourcover-com-covers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-covers-api-openapi.yml
- filename: beyourcover-com-jobs-api-openapi.yml
  format: yaml
  label: BeYourCover Jobs API
  slug: beyourcover-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-jobs-api-openapi.yml
- filename: beyourcover-com-service-api-openapi.yml
  format: yaml
  label: BeYourCover Service API
  slug: beyourcover-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-service-api-openapi.yml
- filename: beyourcover-com-templates-api-openapi.yml
  format: yaml
  label: BeYourCover Templates API
  slug: beyourcover-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-templates-api-openapi.yml
- filename: beyourcover-com-wraps-api-openapi.yml
  format: yaml
  label: BeYourCover Wraps API
  slug: beyourcover-com-wraps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-wraps-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beyourcover.com
  spf: true
hosts:
- cert_expires: Jan  2 07:50:27 2027 GMT
  host: beyourcover.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BeYourCover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeYourCover, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BeYourCover
provider_slug: beyourcover-com
slug: beyourcover-com-domain-security
source_filename: beyourcover-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beyourcover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 07:50:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beyourcover.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/beyourcover-com/security/beyourcover-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- BookCover
- Design
- Publishing
---
