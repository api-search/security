---
api_specs:
- filename: mycase-open-api-openapi.yml
  format: yaml
  label: MyCase Open API
  slug: open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/openapi/mycase-open-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 128 issue "amazon.com"
  - 128 issuewild "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mycase.com
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@stoplight.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Sep 20 18:50:56 2026 GMT
  host: www.mycase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: mycaseapi.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.mycase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mycase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyCase, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MyCase
provider_slug: mycase
slug: mycase-domain-security
source_filename: mycase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mycase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:50:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mycaseapi.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mycase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mycase.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 128 issue \"amazon.com\"\n  - 128 issuewild \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mycase/refs/heads/main/security/mycase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Calendaring
- Case Management
- Client Portal
- Document Management
- Invoicing
- Law Firms
- Legal
- Legal Practice Management
- LegalTech
- Matter Management
- OAuth 2.0
- Payments
- Practice Management
- Time Tracking
- Webhooks
---
