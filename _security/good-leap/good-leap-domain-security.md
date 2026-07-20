---
api_specs:
- filename: good-leap-developer-api-openapi.yml
  format: yaml
  label: GoodLeap Developer API
  slug: goodleap-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-developer-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@goodleap.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goodleap.com
  spf: true
hosts:
- cert_expires: Oct 11 05:42:48 2026 GMT
  host: www.goodleap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.goodleap.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: sandbox01-api.goodleap.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Good Leap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Good Leap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Good Leap
provider_slug: good-leap
slug: good-leap-domain-security
source_filename: good-leap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.goodleap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox01-api.goodleap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: goodleap.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@goodleap.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/security/good-leap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financing
- Lending
- Solar
- Home Improvement
- Sustainability
- Point of Sale
- Loans
- Payments
---
