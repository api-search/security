---
api_specs:
- filename: killbill-api-openapi.json
  format: json
  label: Kill Bill Api API
  slug: kill-bill-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/killbill/openapi/_original/killbill-api-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: killbill.io
  spf: true
hosts:
- cert_expires: Jan 12 21:41:53 2027 GMT
  host: killbill.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kill Bill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kill Bill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kill Bill
provider_slug: killbill
slug: killbill-domain-security
source_filename: killbill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: killbill.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 21:41:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: killbill.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/killbill/security/killbill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Payments
- Subscription Billing
- Usage Metering
- Open Source
- Enterprise Revenue Platform
- Fintech
---
