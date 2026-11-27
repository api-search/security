---
api_specs:
- filename: openapi.json
  format: json
  label: Bankstatemently API
  slug: bankstatemently-api
  spec_type: OpenAPI
  url: https://api.bankstatemently.com/v1/openapi.json
- filename: bankstatemently-com-v1-openapi.json
  format: json
  label: Bankstatemently API V1 API
  slug: bankstatemently-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankstatemently-com/openapi/_original/bankstatemently-com-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bankstatemently.com
  spf: true
hosts:
- cert_expires: Jan  1 01:34:42 2027 GMT
  host: bankstatemently.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bankstatemently Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bankstatemently, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bankstatemently
provider_slug: bankstatemently-com
slug: bankstatemently-com-domain-security
source_filename: bankstatemently-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bankstatemently.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 01:34:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bankstatemently.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bankstatemently-com/security/bankstatemently-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Banking
- Data Conversion
- Software-as-a-Service
---
