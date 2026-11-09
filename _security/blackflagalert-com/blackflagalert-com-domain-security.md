---
api_specs:
- filename: blackflagalert-com-api-openapi.json
  format: json
  label: Black Flag Alert Open API v2 API
  slug: black-flag-alert-open-api-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blackflagalert-com/openapi/_original/blackflagalert-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blackflagalert.com
  spf: true
hosts:
- cert_expires: Jan 22 01:26:17 2027 GMT
  host: blackflagalert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blackflagalert Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Flag Alert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Black Flag Alert
provider_slug: blackflagalert-com
slug: blackflagalert-com-domain-security
source_filename: blackflagalert-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackflagalert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 01:26:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blackflagalert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/blackflagalert-com/security/blackflagalert-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Credit Intelligence
- Company Data
- Risk Scoring
- UK Companies
- Financial Services
---
