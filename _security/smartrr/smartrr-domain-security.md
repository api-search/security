---
api_specs:
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Subscriptions API
  slug: smartrr-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Subscribers API
  slug: smartrr-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Orders and Bills API
  slug: smartrr-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Plans and Purchasables API
  slug: smartrr-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Webhooks API
  slug: smartrr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
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
  dmarc_policy: quarantine
  dnssec: true
  domain: smartrr.com
  spf: true
hosts:
- cert_expires: Sep 29 04:58:06 2026 GMT
  host: smartrr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 20:34:15 2026 GMT
  host: api.smartrr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 05:18:25 2026 GMT
  host: help.smartrr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartrr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartrr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Smartrr
provider_slug: smartrr
slug: smartrr-domain-security
source_filename: smartrr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartrr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:58:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smartrr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 20:34:15 2026 GMT\n  hsts: false\n- host: help.smartrr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 05:18:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smartrr.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/security/smartrr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Subscriptions
- Loyalty
- Shopify
- Ecommerce
- DTC
- Recurring Revenue
- Subscription Management
---
