---
api_specs:
- filename: audito-lat-audit-api-openapi.yml
  format: yaml
  label: audito-lat Audit API
  slug: audito-lat-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audito-lat/openapi/audito-lat-audit-api-openapi.yml
- filename: audito-lat-deep-api-openapi.yml
  format: yaml
  label: audito-lat Deep API
  slug: audito-lat-deep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audito-lat/openapi/audito-lat-deep-api-openapi.yml
- filename: audito-lat-report-api-openapi.yml
  format: yaml
  label: audito-lat Report API
  slug: audito-lat-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audito-lat/openapi/audito-lat-report-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: audito.lat
  spf: true
hosts:
- cert_expires: Jan 12 01:29:21 2027 GMT
  host: audito.lat
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audito Lat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for audito-lat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: audito-lat
provider_slug: audito-lat
slug: audito-lat-domain-security
source_filename: audito-lat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audito.lat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 01:29:21 2027 GMT\n  hsts: null\ndomains:\n- domain: audito.lat\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/audito-lat/security/audito-lat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
