---
api_specs:
- filename: postman-freeagent-api-collection
  format: yaml
  label: FreeAgent REST API
  slug: rest-api
  spec_type: Postman
  url: https://github.com/fac/postman-freeagent-api-collection
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@freeagent.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freeagent.com
  spf: true
hosts:
- cert_expires: Oct  3 00:04:31 2026 GMT
  host: www.freeagent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: dev.freeagent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.freeagent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freeagent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeAgent, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FreeAgent
provider_slug: freeagent
slug: freeagent-domain-security
source_filename: freeagent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freeagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:04:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.freeagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.freeagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freeagent.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@freeagent.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeagent/refs/heads/main/security/freeagent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Small Business
- Invoicing
- Bookkeeping
- Expenses
- Payroll
- VAT
- HMRC
- Making Tax Digital
---
