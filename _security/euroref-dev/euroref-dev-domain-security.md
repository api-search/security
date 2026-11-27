---
api_specs:
- filename: euroref-dev-alerts-api-openapi.yml
  format: yaml
  label: Euroref Alerts API
  slug: euroref-dev-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-alerts-api-openapi.yml
- filename: euroref-dev-answers-api-openapi.yml
  format: yaml
  label: Euroref Answers API
  slug: euroref-dev-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-answers-api-openapi.yml
- filename: euroref-dev-certified-api-openapi.yml
  format: yaml
  label: Euroref Certified API
  slug: euroref-dev-certified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-certified-api-openapi.yml
- filename: euroref-dev-discovery-api-openapi.yml
  format: yaml
  label: Euroref Discovery API
  slug: euroref-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-discovery-api-openapi.yml
- filename: euroref-dev-free-api-openapi.yml
  format: yaml
  label: Euroref Free API
  slug: euroref-dev-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-free-api-openapi.yml
- filename: euroref-dev-jobs-api-openapi.yml
  format: yaml
  label: Euroref Jobs API
  slug: euroref-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-jobs-api-openapi.yml
- filename: euroref-dev-keys-api-openapi.yml
  format: yaml
  label: Euroref Keys API
  slug: euroref-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-keys-api-openapi.yml
- filename: euroref-dev-reference-data-api-openapi.yml
  format: yaml
  label: Euroref Reference data API
  slug: euroref-dev-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-reference-data-api-openapi.yml
- filename: euroref-dev-x402-sellers-api-openapi.yml
  format: yaml
  label: Euroref x402 sellers API
  slug: euroref-dev-x402-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/euroref-dev/openapi/euroref-dev-x402-sellers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: euroref.dev
  spf: true
hosts:
- cert_expires: Dec 11 18:12:25 2026 GMT
  host: euroref.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Euroref Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Euroref, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Euroref
provider_slug: euroref-dev
slug: euroref-dev-domain-security
source_filename: euroref-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: euroref.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 18:12:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: euroref.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/euroref-dev/security/euroref-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Reference Data
- Government
- Europe
- Open Data
---
