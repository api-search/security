---
api_specs:
- filename: mynto-no-bank-api-openapi.yml
  format: yaml
  label: Mynto Bank API
  slug: mynto-no-bank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mynto-no/openapi/mynto-no-bank-api-openapi.yml
- filename: mynto-no-invoicing-api-openapi.yml
  format: yaml
  label: Mynto Invoicing API
  slug: mynto-no-invoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mynto-no/openapi/mynto-no-invoicing-api-openapi.yml
- filename: mynto-no-ledger-api-openapi.yml
  format: yaml
  label: Mynto Ledger API
  slug: mynto-no-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mynto-no/openapi/mynto-no-ledger-api-openapi.yml
- filename: mynto-no-webhooks-api-openapi.yml
  format: yaml
  label: Mynto Webhooks API
  slug: mynto-no-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mynto-no/openapi/mynto-no-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mynto.no
  spf: false
hosts:
- cert_expires: Dec 19 21:53:53 2026 GMT
  host: mynto.no
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mynto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mynto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Mynto
provider_slug: mynto-no
slug: mynto-no-domain-security
source_filename: mynto-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mynto.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 21:53:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mynto.no\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mynto-no/security/mynto-no-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Accounting
- Automation
- Finance
- Software-as-a-Service
- Norway
---
