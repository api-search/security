---
api_specs:
- filename: bitrefill-account-api-openapi.yml
  format: yaml
  label: Bitrefill Account API
  slug: bitrefill-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-account-api-openapi.yml
- filename: bitrefill-checkout-api-openapi.yml
  format: yaml
  label: Bitrefill Checkout API
  slug: bitrefill-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-checkout-api-openapi.yml
- filename: bitrefill-discovery-api-openapi.yml
  format: yaml
  label: Bitrefill Discovery API
  slug: bitrefill-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-discovery-api-openapi.yml
- filename: bitrefill-payments-api-openapi.yml
  format: yaml
  label: Bitrefill Payments API
  slug: bitrefill-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-payments-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bitrefill.com
  spf: true
hosts:
- cert_expires: Jan 27 13:19:49 2027 GMT
  host: www.bitrefill.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitrefill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitrefill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bitrefill
provider_slug: bitrefill
slug: bitrefill-domain-security
source_filename: bitrefill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitrefill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 13:19:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitrefill.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bitrefill/security/bitrefill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Payments
- Gift Cards
- Mobile Top-Up
---
