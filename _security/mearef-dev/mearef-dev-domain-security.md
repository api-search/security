---
api_specs:
- filename: mearef-dev-alerts-api-openapi.yml
  format: yaml
  label: Mearef Alerts API
  slug: mearef-dev-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-alerts-api-openapi.yml
- filename: mearef-dev-answers-api-openapi.yml
  format: yaml
  label: Mearef Answers API
  slug: mearef-dev-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-answers-api-openapi.yml
- filename: mearef-dev-certified-api-openapi.yml
  format: yaml
  label: Mearef Certified API
  slug: mearef-dev-certified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-certified-api-openapi.yml
- filename: mearef-dev-discovery-api-openapi.yml
  format: yaml
  label: Mearef Discovery API
  slug: mearef-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-discovery-api-openapi.yml
- filename: mearef-dev-free-api-openapi.yml
  format: yaml
  label: Mearef Free API
  slug: mearef-dev-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-free-api-openapi.yml
- filename: mearef-dev-jobs-api-openapi.yml
  format: yaml
  label: Mearef Jobs API
  slug: mearef-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-jobs-api-openapi.yml
- filename: mearef-dev-keys-api-openapi.yml
  format: yaml
  label: Mearef Keys API
  slug: mearef-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-keys-api-openapi.yml
- filename: mearef-dev-reference-data-api-openapi.yml
  format: yaml
  label: Mearef Reference data API
  slug: mearef-dev-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-reference-data-api-openapi.yml
- filename: mearef-dev-x402-sellers-api-openapi.yml
  format: yaml
  label: Mearef x402 sellers API
  slug: mearef-dev-x402-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-x402-sellers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mearef.dev
  spf: true
hosts:
- cert_expires: Dec 20 13:36:05 2026 GMT
  host: mearef.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mearef Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mearef, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mearef
provider_slug: mearef-dev
slug: mearef-dev-domain-security
source_filename: mearef-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mearef.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 13:36:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mearef.dev\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mearef-dev/security/mearef-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Government
- Middle East
---
