---
api_specs:
- filename: galaxyunit-app-actions-api-openapi.yml
  format: yaml
  label: Galaxy Unit Actions API
  slug: galaxyunit-app-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-actions-api-openapi.yml
- filename: galaxyunit-app-business-api-openapi.yml
  format: yaml
  label: Galaxy Unit Business API
  slug: galaxyunit-app-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-business-api-openapi.yml
- filename: galaxyunit-app-contacts-api-openapi.yml
  format: yaml
  label: Galaxy Unit Contacts API
  slug: galaxyunit-app-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-contacts-api-openapi.yml
- filename: galaxyunit-app-estimate-api-openapi.yml
  format: yaml
  label: Galaxy Unit Estimate API
  slug: galaxyunit-app-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-estimate-api-openapi.yml
- filename: galaxyunit-app-events-api-openapi.yml
  format: yaml
  label: Galaxy Unit Events API
  slug: galaxyunit-app-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-events-api-openapi.yml
- filename: galaxyunit-app-expenses-api-openapi.yml
  format: yaml
  label: Galaxy Unit Expenses API
  slug: galaxyunit-app-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-expenses-api-openapi.yml
- filename: galaxyunit-app-invoices-api-openapi.yml
  format: yaml
  label: Galaxy Unit Invoices API
  slug: galaxyunit-app-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-invoices-api-openapi.yml
- filename: galaxyunit-app-jobs-api-openapi.yml
  format: yaml
  label: Galaxy Unit Jobs API
  slug: galaxyunit-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-jobs-api-openapi.yml
- filename: galaxyunit-app-me-api-openapi.yml
  format: yaml
  label: Galaxy Unit Me API
  slug: galaxyunit-app-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-me-api-openapi.yml
- filename: galaxyunit-app-quotes-api-openapi.yml
  format: yaml
  label: Galaxy Unit Quotes API
  slug: galaxyunit-app-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-quotes-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: galaxyunit.app
  spf: true
hosts:
- cert_expires: Jan 15 08:29:19 2027 GMT
  host: galaxyunit.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Galaxy Unit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galaxy Unit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Galaxy Unit
provider_slug: galaxyunit-app
slug: galaxyunit-app-domain-security
source_filename: galaxyunit-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: galaxyunit.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 08:29:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: galaxyunit.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/galaxyunit-app/security/galaxyunit-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business
- Software-as-a-Service
- ServiceIndustry
- Artificial Intelligence
---
