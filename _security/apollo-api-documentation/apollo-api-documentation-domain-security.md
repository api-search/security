---
api_specs:
- filename: apollo-api-documentation-openapi.yml
  format: yaml
  label: Apollo REST API
  slug: apollo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-openapi.yml
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
  dmarc_policy: reject
  dnssec: false
  domain: apollo.io
  spf: true
hosts:
- cert_expires: Oct  3 09:31:14 2026 GMT
  host: docs.apollo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 12:03:29 2026 GMT
  host: api.apollo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apollo Api Documentation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo API Documentation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apollo API Documentation
provider_slug: apollo-api-documentation
slug: apollo-api-documentation-domain-security
source_filename: apollo-api-documentation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:03:29 2026 GMT\n  hsts: null\ndomains:\n- domain: apollo.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/security/apollo-api-documentation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Documentation
- Best Practices
- Data Enrichment
- People Search
- Sales Intelligence
---
