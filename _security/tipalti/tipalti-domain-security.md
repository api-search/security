---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Tipalti REST API
  slug: tipalti-rest-api
  spec_type: OpenAPI
  url: https://developer.tipalti.com/
description: ''
domains:
- caa:
  - 0 issue "infocert.it"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@tipalti.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tipalti.com
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: tipalti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: developer.tipalti.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.tipalti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tipalti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tipalti, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tipalti
provider_slug: tipalti
slug: tipalti-domain-security
source_filename: tipalti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tipalti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tipalti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.tipalti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tipalti.com\n  dnssec: false\n  caa:\n  - 0 issue \"infocert.it\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@tipalti.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tipalti/refs/heads/main/security/tipalti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounts Payable
- Mass Payments
- Global Payments
- Payee Onboarding
- Invoice Management
- Tax Compliance
- Procurement
- Financial Automation
- Fintech
- B2B Payments
---
