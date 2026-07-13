---
api_specs:
- filename: chargedesk-rest-api-openapi.yml
  format: yaml
  label: ChargeDesk REST API
  slug: chargedesk-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/openapi/chargedesk-rest-api-openapi.yml
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
  dmarc_policy: quarantine
  dnssec: true
  domain: chargedesk.com
  spf: true
hosts:
- cert_expires: Oct  6 13:31:34 2026 GMT
  host: chargedesk.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 00:50:28 2026 GMT
  host: api.chargedesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chargedesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChargeDesk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ChargeDesk
provider_slug: chargedesk
slug: chargedesk-domain-security
source_filename: chargedesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chargedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.chargedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:50:28 2026 GMT\n  hsts: null\ndomains:\n- domain: chargedesk.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/security/chargedesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Billing
- Subscriptions
- Charges
- Refunds
- Customer Management
- Payment Gateway
- Helpdesk Integration
- REST API
---
