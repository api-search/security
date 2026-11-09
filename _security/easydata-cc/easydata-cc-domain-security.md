---
api_specs:
- filename: easydata-cc-openapi-generated.yml
  format: yaml
  label: EasyData API
  slug: easydata-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easydata-cc/openapi/_ae-authored/easydata-cc-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: easydata.cc
  spf: true
hosts:
- cert_expires: Jan 18 09:21:12 2027 GMT
  host: easydata.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easydata Cc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EasyData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: EasyData
provider_slug: easydata-cc
slug: easydata-cc-domain-security
source_filename: easydata-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easydata.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 09:21:12 2027 GMT\n  hsts: false\ndomains:\n- domain: easydata.cc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/easydata-cc/security/easydata-cc-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Data Management
- Artificial Intelligence
- Spreadsheets
- Collaboration
- Software-as-a-Service
---
