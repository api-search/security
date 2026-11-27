---
api_specs:
- filename: latamref-dev-alerts-api-openapi.yml
  format: yaml
  label: Latamref Alerts API
  slug: latamref-dev-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-alerts-api-openapi.yml
- filename: latamref-dev-answers-api-openapi.yml
  format: yaml
  label: Latamref Answers API
  slug: latamref-dev-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-answers-api-openapi.yml
- filename: latamref-dev-certified-api-openapi.yml
  format: yaml
  label: Latamref Certified API
  slug: latamref-dev-certified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-certified-api-openapi.yml
- filename: latamref-dev-discovery-api-openapi.yml
  format: yaml
  label: Latamref Discovery API
  slug: latamref-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-discovery-api-openapi.yml
- filename: latamref-dev-free-api-openapi.yml
  format: yaml
  label: Latamref Free API
  slug: latamref-dev-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-free-api-openapi.yml
- filename: latamref-dev-jobs-api-openapi.yml
  format: yaml
  label: Latamref Jobs API
  slug: latamref-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-jobs-api-openapi.yml
- filename: latamref-dev-keys-api-openapi.yml
  format: yaml
  label: Latamref Keys API
  slug: latamref-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-keys-api-openapi.yml
- filename: latamref-dev-reference-data-api-openapi.yml
  format: yaml
  label: Latamref Reference data API
  slug: latamref-dev-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-reference-data-api-openapi.yml
- filename: latamref-dev-x402-sellers-api-openapi.yml
  format: yaml
  label: Latamref x402 sellers API
  slug: latamref-dev-x402-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-x402-sellers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: latamref.dev
  spf: true
hosts:
- cert_expires: Feb  8 19:31:29 2027 GMT
  host: latamref.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Latamref Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latamref, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Latamref
provider_slug: latamref-dev
slug: latamref-dev-domain-security
source_filename: latamref-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latamref.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 19:31:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: latamref.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/latamref-dev/security/latamref-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data
- Government
- Latin America
- Reference
---
