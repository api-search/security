---
api_specs:
- filename: easyparser-com-amazon-api-openapi.yml
  format: yaml
  label: easyparser-com Amazon API
  slug: easyparser-com-amazon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyparser-com/openapi/easyparser-com-amazon-api-openapi.yml
- filename: easyparser-com-bulk-api-openapi.yml
  format: yaml
  label: easyparser-com Bulk API
  slug: easyparser-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyparser-com/openapi/easyparser-com-bulk-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easyparser.com
  spf: true
hosts:
- cert_expires: Dec 23 13:36:48 2026 GMT
  host: easyparser.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easyparser Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for easyparser-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: easyparser-com
provider_slug: easyparser-com
slug: easyparser-com-domain-security
source_filename: easyparser-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easyparser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 13:36:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: easyparser.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/easyparser-com/security/easyparser-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Amazon
- Scraping
- Real-time
- Data-Extraction
---
