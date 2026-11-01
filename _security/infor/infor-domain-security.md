---
api_specs:
- filename: infor-contents-api-openapi.yml
  format: yaml
  label: Infor Contents API
  slug: infor-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-contents-api-openapi.yml
- filename: infor-icua-api-openapi.yml
  format: yaml
  label: Infor ICUA API
  slug: infor-icua-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-icua-api-openapi.yml
- filename: infor-languages-api-openapi.yml
  format: yaml
  label: Infor Languages API
  slug: infor-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-languages-api-openapi.yml
- filename: infor-products-api-openapi.yml
  format: yaml
  label: Infor Products API
  slug: infor-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-products-api-openapi.yml
- filename: infor-recenttopics-api-openapi.yml
  format: yaml
  label: Infor Recent Topics API
  slug: infor-recenttopics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-recenttopics-api-openapi.yml
- filename: infor-s3-docs-api-openapi.yml
  format: yaml
  label: Infor S3 Docs API
  slug: infor-s3-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-s3-docs-api-openapi.yml
- filename: infor-search-api-openapi.yml
  format: yaml
  label: Infor Search API
  slug: infor-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-search-api-openapi.yml
- filename: infor-security-api-openapi.yml
  format: yaml
  label: Infor Security API
  slug: infor-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-security-api-openapi.yml
- filename: infor-solutions-api-openapi.yml
  format: yaml
  label: Infor Solutions API
  slug: infor-solutions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-solutions-api-openapi.yml
- filename: infor-userfavorites-api-openapi.yml
  format: yaml
  label: Infor User Favorites API
  slug: infor-userfavorites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-userfavorites-api-openapi.yml
- filename: infor-web-api-openapi.yml
  format: yaml
  label: Infor Web API
  slug: infor-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infor/openapi/infor-web-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: infor.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.infor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.infor.com
  https: false
- host: mingledev01-ionapi.mingle.infor.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Infor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infor, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Infor
provider_slug: infor
slug: infor-domain-security
source_filename: infor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.infor.com\n  https: false\n- host: mingledev01-ionapi.mingle.infor.com\n  https: false\ndomains:\n- domain: infor.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/infor/security/infor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ERP
- Manufacturing
- Supply Chain
- Cloud
- Integration
---
