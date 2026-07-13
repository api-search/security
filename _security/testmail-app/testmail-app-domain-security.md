---
api_specs:
- filename: testmail-app-json-api-openapi.yml
  format: yaml
  label: Testmail JSON API
  slug: testmail-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/openapi/testmail-app-json-api-openapi.yml
- filename: testmail-app-graphql-api-openapi.yml
  format: yaml
  label: Testmail GraphQL API
  slug: testmail-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/openapi/testmail-app-graphql-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: testmail.app
  spf: true
hosts:
- cert_expires: Oct  1 01:11:14 2026 GMT
  host: testmail.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 16:05:20 2026 GMT
  host: api.testmail.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Testmail App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Testmail, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Testmail
provider_slug: testmail-app
slug: testmail-app-domain-security
source_filename: testmail-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: testmail.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:11:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.testmail.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:05:20 2026 GMT\n  hsts: null\ndomains:\n- domain: testmail.app\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/security/testmail-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Testing
- Developer Tools
- API Testing
- GraphQL
- REST API
- CI/CD
- QA Automation
- Programmable Inboxes
---
