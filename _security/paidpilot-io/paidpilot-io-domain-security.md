---
api_specs:
- filename: paidpilot-io-invoice-from-timesheet-api-openapi.yml
  format: yaml
  label: PaidPilot Invoice From Timesheet API
  slug: paidpilot-io-invoice-from-timesheet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidpilot-io/openapi/paidpilot-io-invoice-from-timesheet-api-openapi.yml
- filename: paidpilot-io-invoice-pdf-api-openapi.yml
  format: yaml
  label: PaidPilot Invoice.pdf API
  slug: paidpilot-io-invoice-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidpilot-io/openapi/paidpilot-io-invoice-pdf-api-openapi.yml
- filename: paidpilot-io-late-fee-api-openapi.yml
  format: yaml
  label: PaidPilot Late Fee API
  slug: paidpilot-io-late-fee-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidpilot-io/openapi/paidpilot-io-late-fee-api-openapi.yml
- filename: paidpilot-io-payment-terms-api-openapi.yml
  format: yaml
  label: PaidPilot Payment Terms API
  slug: paidpilot-io-payment-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidpilot-io/openapi/paidpilot-io-payment-terms-api-openapi.yml
- filename: paidpilot-io-receivables-report-api-openapi.yml
  format: yaml
  label: PaidPilot Receivables Report API
  slug: paidpilot-io-receivables-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidpilot-io/openapi/paidpilot-io-receivables-report-api-openapi.yml
- filename: paidpilot-io-reminder-draft-api-openapi.yml
  format: yaml
  label: PaidPilot Reminder Draft API
  slug: paidpilot-io-reminder-draft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidpilot-io/openapi/paidpilot-io-reminder-draft-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paidpilot.io
  spf: false
hosts:
- cert_expires: Jan 17 21:34:22 2027 GMT
  host: paidpilot.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PaidPilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PaidPilot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: PaidPilot
provider_slug: paidpilot-io
slug: paidpilot-io-domain-security
source_filename: paidpilot-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paidpilot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 21:34:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paidpilot.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/paidpilot-io/security/paidpilot-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Invoicing
- Privacy
---
