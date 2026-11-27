---
api_specs:
- filename: tesseralytics-dev-catalog-api-openapi.yml
  format: yaml
  label: Tessera Analytics Catalog API
  slug: tesseralytics-dev-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tesseralytics-dev/openapi/tesseralytics-dev-catalog-api-openapi.yml
- filename: tesseralytics-dev-datasets-api-openapi.yml
  format: yaml
  label: Tessera Analytics Datasets API
  slug: tesseralytics-dev-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tesseralytics-dev/openapi/tesseralytics-dev-datasets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tesseralytics.dev
  spf: true
hosts:
- cert_expires: May 26 08:09:34 2027 GMT
  host: tesseralytics.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tessera Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tessera Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tessera Analytics
provider_slug: tesseralytics-dev
slug: tesseralytics-dev-domain-security
source_filename: tesseralytics-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tesseralytics.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 26 08:09:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tesseralytics.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tesseralytics-dev/security/tesseralytics-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- MarketData
- Analytics
- API
---
