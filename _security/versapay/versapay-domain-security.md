---
api_specs:
- filename: versapay-api-reference.json
  format: json
  label: Versapay API Reference
  slug: versapay-api-reference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/versapay/refs/heads/main/openapi/versapay-api-reference.json
- filename: versapay-ecommerce-api.json
  format: json
  label: Versapay Ecommerce API
  slug: versapay-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/versapay/refs/heads/main/openapi/versapay-ecommerce-api.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "entrust.net"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: versapay.com
  spf: true
hosts:
- cert_expires: Oct 12 18:22:20 2026 GMT
  host: versapay.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: developers.versapay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:22:20 2026 GMT
  host: secure.versapay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Versapay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Versapay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Versapay
provider_slug: versapay
slug: versapay-domain-security
source_filename: versapay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: versapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:22:20 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developers.versapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\n- host: secure.versapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:22:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: versapay.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/versapay/refs/heads/main/security/versapay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Canada
- Accounts Receivable
- AR Automation
- Order to Cash
- Payment Acceptance
- Payment Processing
- B2B Payments
- Invoicing
- Ecommerce
- Card Present
- Webhooks
---
