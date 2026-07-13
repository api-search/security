---
api_specs:
- filename: paylocity-openapi.yml
  format: yaml
  label: Paylocity Integrations REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paylocity/refs/heads/main/openapi/paylocity-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paylocity.com
  spf: true
hosts:
- cert_expires: Jul 27 01:02:51 2026 GMT
  host: www.paylocity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 02:15:14 2026 GMT
  host: developer.paylocity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: api.paylocity.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Paylocity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paylocity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paylocity
provider_slug: paylocity
slug: paylocity-domain-security
source_filename: paylocity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paylocity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 01:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.paylocity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paylocity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: paylocity.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paylocity/refs/heads/main/security/paylocity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Payroll
- HCM
- Benefits
- Workforce Management
- Time Tracking
---
