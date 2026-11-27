---
api_specs:
- filename: gentender-ru-agent-api-openapi.yml
  format: yaml
  label: GenTender Agent API
  slug: gentender-ru-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentender-ru/openapi/gentender-ru-agent-api-openapi.yml
- filename: gentender-ru-gisp-api-openapi.yml
  format: yaml
  label: GenTender Gisp API
  slug: gentender-ru-gisp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentender-ru/openapi/gentender-ru-gisp-api-openapi.yml
- filename: gentender-ru-predictor-api-openapi.yml
  format: yaml
  label: GenTender Predictor API
  slug: gentender-ru-predictor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentender-ru/openapi/gentender-ru-predictor-api-openapi.yml
- filename: gentender-ru-tenders-api-openapi.yml
  format: yaml
  label: GenTender Tenders API
  slug: gentender-ru-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentender-ru/openapi/gentender-ru-tenders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gentender.ru
  spf: true
hosts:
- cert_expires: Dec 11 03:03:48 2026 GMT
  host: gentender.ru
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GenTender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenTender, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GenTender
provider_slug: gentender-ru
slug: gentender-ru-domain-security
source_filename: gentender-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gentender.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 03:03:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gentender.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gentender-ru/security/gentender-ru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- Procurement
- Artificial Intelligence
- Russian
- Government
---
