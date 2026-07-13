---
api_specs:
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Profiles API
  slug: adapty-server-side-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Purchases & Transactions API
  slug: adapty-server-side-purchases-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Access Levels API
  slug: adapty-server-side-access-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Paywalls & Products API
  slug: adapty-server-side-paywalls-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Integrations API
  slug: adapty-server-side-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adapty.io
  spf: true
hosts:
- cert_expires: Sep 15 08:58:04 2026 GMT
  host: adapty.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:19:53 2026 GMT
  host: api.adapty.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adapty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adapty, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adapty
provider_slug: adapty
slug: adapty-domain-security
source_filename: adapty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adapty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:58:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.adapty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:19:53 2026 GMT\n  hsts: null\ndomains:\n- domain: adapty.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/security/adapty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile
- Subscriptions
- In-App Purchases
- Paywalls
- Analytics
---
