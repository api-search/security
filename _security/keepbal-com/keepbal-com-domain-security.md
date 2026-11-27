---
api_specs:
- filename: keepbal-com-account-api-openapi.yml
  format: yaml
  label: KeepBal Account API
  slug: keepbal-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-account-api-openapi.yml
- filename: keepbal-com-discovery-api-openapi.yml
  format: yaml
  label: KeepBal Discovery API
  slug: keepbal-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-discovery-api-openapi.yml
- filename: keepbal-com-models-api-openapi.yml
  format: yaml
  label: KeepBal Models API
  slug: keepbal-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-models-api-openapi.yml
- filename: keepbal-com-operations-api-openapi.yml
  format: yaml
  label: KeepBal Operations API
  slug: keepbal-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-operations-api-openapi.yml
- filename: keepbal-com-pay-per-request-api-openapi.yml
  format: yaml
  label: KeepBal Pay Per Request API
  slug: keepbal-com-pay-per-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-pay-per-request-api-openapi.yml
- filename: keepbal-com-tools-api-openapi.yml
  format: yaml
  label: KeepBal Tools API
  slug: keepbal-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepbal-com/openapi/keepbal-com-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keepbal.com
  spf: true
hosts:
- cert_expires: Jan  3 09:59:28 2027 GMT
  host: keepbal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KeepBal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeepBal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KeepBal
provider_slug: keepbal-com
slug: keepbal-com-domain-security
source_filename: keepbal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keepbal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 09:59:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keepbal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/keepbal-com/security/keepbal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Gateway
- Tool Integration
- Prepaid Wallet
- Developer Platform
---
