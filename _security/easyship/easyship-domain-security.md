---
api_specs:
- filename: easyship-openapi.yml
  format: yaml
  label: Easyship API
  slug: easyship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-openapi.yml
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
  domain: easyship.com
  spf: true
hosts:
- cert_expires: Sep 19 04:12:23 2026 GMT
  host: www.easyship.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 02:24:31 2026 GMT
  host: developers.easyship.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 04:12:23 2026 GMT
  host: api.easyship.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Easyship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easyship, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Easyship
provider_slug: easyship
slug: easyship-domain-security
source_filename: easyship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.easyship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 04:12:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.easyship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:24:31 2026 GMT\n  hsts: null\n- host: api.easyship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 04:12:23 2026 GMT\n  hsts: null\ndomains:\n- domain: easyship.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/security/easyship-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Shipping
- Logistics
- Ecommerce
- Fulfillment
- CrossBorder
---
