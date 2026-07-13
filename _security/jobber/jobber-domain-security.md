---
api_specs:
- filename: jobber-developer-api-openapi.yml
  format: yaml
  label: Jobber Developer API
  slug: jobber-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobber/refs/heads/main/openapi/jobber-developer-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getjobber.com
  spf: true
hosts:
- cert_expires: Aug 25 07:59:16 2026 GMT
  host: getjobber.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:43:31 2026 GMT
  host: developer.getjobber.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 02:11:39 2026 GMT
  host: api.getjobber.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jobber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobber, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jobber
provider_slug: jobber
slug: jobber-domain-security
source_filename: jobber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getjobber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 07:59:16 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.getjobber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.getjobber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:11:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: getjobber.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobber/refs/heads/main/security/jobber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- Home Service
- Scheduling
- Quoting
- Invoicing
- Dispatching
- Mobile Workforce
- CRM
- SaaS
- GraphQL
---
