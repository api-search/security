---
api_specs:
- filename: mollie-openapi-original.yml
  format: yaml
  label: Mollie API
  slug: mollie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mollie/refs/heads/main/openapi/mollie-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issuewild ";"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mollie.com
  spf: true
hosts:
- cert_expires: Sep 17 10:28:00 2026 GMT
  host: www.mollie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 06:49:02 2026 GMT
  host: docs.mollie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 10:28:00 2026 GMT
  host: api.mollie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mollie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mollie, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mollie
provider_slug: mollie
slug: mollie-domain-security
source_filename: mollie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mollie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:28:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mollie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 06:49:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mollie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:28:00 2026 GMT\n  hsts: null\ndomains:\n- domain: mollie.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mollie/refs/heads/main/security/mollie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Fintech
- Financial Services
- Checkout
- Ecommerce
- Subscriptions
- Point of Sale
- Europe
- Netherlands
---
