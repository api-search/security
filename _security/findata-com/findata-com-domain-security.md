---
api_specs:
- filename: findata-com-companies-api-openapi.yml
  format: yaml
  label: FinData Companies API
  slug: findata-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-companies-api-openapi.yml
- filename: findata-com-corporate-actions-api-openapi.yml
  format: yaml
  label: FinData Corporate actions API
  slug: findata-com-corporate-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-corporate-actions-api-openapi.yml
- filename: findata-com-fundamentals-api-openapi.yml
  format: yaml
  label: FinData Fundamentals API
  slug: findata-com-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-fundamentals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: findata.com
  spf: false
hosts:
- cert_expires: Feb 11 03:38:38 2027 GMT
  host: findata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FinData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FinData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: FinData
provider_slug: findata-com
slug: findata-com-domain-security
source_filename: findata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 03:38:38 2027 GMT\n  hsts: false\ndomains:\n- domain: findata.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/findata-com/security/findata-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Data
- SEC Fundamentals
- Market Data
- Research
---
