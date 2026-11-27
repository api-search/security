---
api_specs:
- filename: fairvalid-com-balance-api-openapi.yml
  format: yaml
  label: FairValid Balance API
  slug: fairvalid-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairvalid-com/openapi/fairvalid-com-balance-api-openapi.yml
- filename: fairvalid-com-fairmatch-api-openapi.yml
  format: yaml
  label: FairValid Fair Match API
  slug: fairvalid-com-fairmatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairvalid-com/openapi/fairvalid-com-fairmatch-api-openapi.yml
- filename: fairvalid-com-jobs-api-openapi.yml
  format: yaml
  label: FairValid Jobs API
  slug: fairvalid-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairvalid-com/openapi/fairvalid-com-jobs-api-openapi.yml
- filename: fairvalid-com-simulator-api-openapi.yml
  format: yaml
  label: FairValid Simulator API
  slug: fairvalid-com-simulator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairvalid-com/openapi/fairvalid-com-simulator-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fairvalid.com
  spf: true
hosts:
- cert_expires: Jan 15 20:14:29 2027 GMT
  host: fairvalid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FairValid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FairValid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FairValid
provider_slug: fairvalid-com
slug: fairvalid-com-domain-security
source_filename: fairvalid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fairvalid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 20:14:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fairvalid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fairvalid-com/security/fairvalid-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Email Verification
- Contact Search
- Sales
- Marketing
---
