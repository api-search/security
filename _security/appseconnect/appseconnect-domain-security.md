---
api_specs:
- filename: appseconnect-openapi-generated.yml
  format: yaml
  label: APPSeCONNECT Corp API
  slug: appseconnect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appseconnect/openapi/_ae-authored/appseconnect-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appseconnect.com
  spf: true
hosts:
- cert_expires: Jan  8 14:11:20 2027 GMT
  host: appseconnect.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appseconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APPSeCONNECT Corp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: APPSeCONNECT Corp
provider_slug: appseconnect
slug: appseconnect-domain-security
source_filename: appseconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appseconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 14:11:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: appseconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/appseconnect/security/appseconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Integration
- iPaaS
- AI
- ERP
---
