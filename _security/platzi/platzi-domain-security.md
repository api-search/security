---
api_specs:
- filename: platzi-fake-store-openapi-original.json
  format: json
  label: Platzi Fake Store API
  slug: platzi-fake-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platzi/refs/heads/main/openapi/platzi-fake-store-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: platzi.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: escuelajs.co
  spf: true
hosts:
- cert_expires: Oct 10 07:58:46 2026 GMT
  host: fakeapi.platzi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 01:07:33 2026 GMT
  host: api.escuelajs.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Platzi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Platzi, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Platzi
provider_slug: platzi
slug: platzi-domain-security
source_filename: platzi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fakeapi.platzi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 07:58:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.escuelajs.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:07:33 2026 GMT\n  hsts: null\ndomains:\n- domain: platzi.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: escuelajs.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platzi/refs/heads/main/security/platzi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- E-Commerce
- Products
- Mock API
- Prototyping
- REST
- GraphQL
- Fake Store
- Developer Tools
---
