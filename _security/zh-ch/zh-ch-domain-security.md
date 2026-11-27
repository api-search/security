---
api_specs:
- filename: zh-ch-collector-configuration-api-openapi.yml
  format: yaml
  label: Kanton Zürich Collector configuration API
  slug: zh-ch-collector-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-collector-configuration-api-openapi.yml
- filename: zh-ch-collector-state-api-openapi.yml
  format: yaml
  label: Kanton Zürich Collector state API
  slug: zh-ch-collector-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-collector-state-api-openapi.yml
- filename: zh-ch-funktional-api-openapi.yml
  format: yaml
  label: Kanton Zürich Funktional API
  slug: zh-ch-funktional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-funktional-api-openapi.yml
- filename: zh-ch-online-data-api-openapi.yml
  format: yaml
  label: Kanton Zürich Online Data API
  slug: zh-ch-online-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-online-data-api-openapi.yml
- filename: zh-ch-tests-api-openapi.yml
  format: yaml
  label: Kanton Zürich Tests API
  slug: zh-ch-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zh-ch/openapi/zh-ch-tests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zh.ch
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.zh.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kanton Zürich Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kanton Zürich, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kanton Zürich
provider_slug: zh-ch
slug: zh-ch-domain-security
source_filename: zh-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zh.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zh.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zh-ch/security/zh-ch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Open Data
- Switzerland
- Statistics
- Traffic
- Education
- Geodata
---
