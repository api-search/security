---
api_specs:
- filename: capmonster-account-api-openapi.yml
  format: yaml
  label: Capmonster Account API
  slug: capmonster-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capmonster/openapi/capmonster-account-api-openapi.yml
- filename: capmonster-tasks-api-openapi.yml
  format: yaml
  label: Capmonster Tasks API
  slug: capmonster-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capmonster/openapi/capmonster-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: capmonster.cloud
  spf: true
hosts:
- cert_expires: Jan  2 05:58:47 2027 GMT
  host: capmonster.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capmonster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capmonster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Capmonster
provider_slug: capmonster
slug: capmonster-domain-security
source_filename: capmonster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capmonster.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 05:58:47 2027 GMT\n  hsts: false\ndomains:\n- domain: capmonster.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/capmonster/security/capmonster-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- CAPTCHA
- AI
- Automation
- Cloud
---
