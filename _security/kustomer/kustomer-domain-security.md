---
api_specs:
- filename: kustomer-openapi.yml
  format: yaml
  label: Kustomer REST API
  slug: kustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kustomer/refs/heads/main/openapi/kustomer-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:devops+caa@kustomer.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kustomer.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kustomerapp.com
  spf: true
hosts:
- cert_expires: Oct  9 01:18:02 2026 GMT
  host: www.kustomer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:09:06 2026 GMT
  host: developer.kustomer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.kustomerapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kustomer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kustomer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kustomer
provider_slug: kustomer
slug: kustomer-domain-security
source_filename: kustomer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kustomer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.kustomer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:09:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kustomerapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kustomer.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:devops+caa@kustomer.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kustomerapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kustomer/refs/heads/main/security/kustomer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Customer Service
- CRM
- Helpdesk
- Messaging
- AI
---
