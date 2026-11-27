---
api_specs:
- filename: futbolatlas-app-corpus-api-openapi.yml
  format: yaml
  label: Football Atlas Corpus API
  slug: futbolatlas-app-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/futbolatlas-app/openapi/futbolatlas-app-corpus-api-openapi.yml
- filename: futbolatlas-app-deployment-api-openapi.yml
  format: yaml
  label: Football Atlas Deployment API
  slug: futbolatlas-app-deployment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/futbolatlas-app/openapi/futbolatlas-app-deployment-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: futbolatlas.app
  spf: false
hosts:
- cert_expires: Jan 15 18:07:41 2027 GMT
  host: futbolatlas.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Football Atlas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Football Atlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Football Atlas
provider_slug: futbolatlas-app
slug: futbolatlas-app-domain-security
source_filename: futbolatlas-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: futbolatlas.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 18:07:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: futbolatlas.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/futbolatlas-app/security/futbolatlas-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Football
- Sports
- Knowledge Base
- Data
- Open Data
---
