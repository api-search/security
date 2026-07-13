---
api_specs:
- filename: housecall-pro-public-api-openapi.yml
  format: yaml
  label: Housecall Pro Public API
  slug: housecall-pro-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housecall-pro/refs/heads/main/openapi/housecall-pro-public-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: housecallpro.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.housecallpro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 19:33:28 2026 GMT
  host: docs.housecallpro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.housecallpro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Housecall Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Housecall Pro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Housecall Pro
provider_slug: housecall-pro
slug: housecall-pro-domain-security
source_filename: housecall-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.housecallpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\n- host: docs.housecallpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:33:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.housecallpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: housecallpro.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/housecall-pro/refs/heads/main/security/housecall-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Home Services
- Field Service Management
- Scheduling
- Dispatching
- Invoicing
- Payments
- HVAC
- Plumbing
- Electrical
- Cleaning
- Landscaping
- Pest Control
- SaaS
---
