---
api_specs:
- filename: myopc-io-accounting-api-openapi.yml
  format: yaml
  label: OPC Suite Accounting API
  slug: myopc-io-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-accounting-api-openapi.yml
- filename: myopc-io-crm-api-openapi.yml
  format: yaml
  label: OPC Suite CRM API
  slug: myopc-io-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-crm-api-openapi.yml
- filename: myopc-io-hr-api-openapi.yml
  format: yaml
  label: OPC Suite HR API
  slug: myopc-io-hr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-hr-api-openapi.yml
- filename: myopc-io-inventory-api-openapi.yml
  format: yaml
  label: OPC Suite Inventory API
  slug: myopc-io-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-inventory-api-openapi.yml
- filename: myopc-io-sales-api-openapi.yml
  format: yaml
  label: OPC Suite Sales API
  slug: myopc-io-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-sales-api-openapi.yml
- filename: myopc-io-work-api-openapi.yml
  format: yaml
  label: OPC Suite Work API
  slug: myopc-io-work-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-work-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: myopc.io
  spf: false
hosts:
- cert_expires: Feb  3 08:44:59 2027 GMT
  host: myopc.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OPC Suite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OPC Suite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OPC Suite
provider_slug: myopc-io
slug: myopc-io-domain-security
source_filename: myopc-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myopc.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:44:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: myopc.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/myopc-io/security/myopc-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- ERP
- CRM
- Artificial Intelligence
- Business Management
- Software-as-a-Service
---
