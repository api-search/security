---
api_specs:
- filename: omophub-openapi-generated.yml
  format: yaml
  label: OMOPHub API
  slug: omophub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omophub/openapi/_ae-authored/omophub-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: omophub.com
  spf: true
hosts:
- cert_expires: Jan  6 01:16:01 2027 GMT
  host: omophub.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Omophub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OMOPHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OMOPHub
provider_slug: omophub
slug: omophub-domain-security
source_filename: omophub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omophub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 01:16:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: omophub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/omophub/security/omophub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Data Integration
- OMOP
- APIs
---
