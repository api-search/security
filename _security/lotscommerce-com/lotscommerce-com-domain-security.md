---
api_specs:
- filename: lotscommerce-com-openapi-generated.yml
  format: yaml
  label: LotsStore API
  slug: lotscommerce-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lotscommerce-com/openapi/_ae-authored/lotscommerce-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: lotscommerce.com
  spf: false
hosts:
- cert_expires: Jan  7 07:06:36 2027 GMT
  host: lotscommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LotsStore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LotsStore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LotsStore
provider_slug: lotscommerce-com
slug: lotscommerce-com-domain-security
source_filename: lotscommerce-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lotscommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 07:06:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lotscommerce.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lotscommerce-com/security/lotscommerce-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- E-Commerce
- Software-as-a-Service
- Store Builder
- Low Commission
---
