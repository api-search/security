---
api_specs:
- filename: target-target-api-openapi.yml
  format: yaml
  label: Target API
  slug: target-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-target-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:certificate.management@target.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: target.com
  spf: true
hosts:
- cert_expires: Oct  6 16:25:18 2026 GMT
  host: www.target.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 16:25:18 2026 GMT
  host: developer.target.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 15:20:11 2026 GMT
  host: api.target.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Target Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for target, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: target
provider_slug: target
slug: target-domain-security
source_filename: target-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:25:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:25:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 15:20:11 2026 GMT\n  hsts: null\ndomains:\n- domain: target.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:certificate.management@target.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/security/target-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- E-Commerce
- Retail
- Products
- Inventory
- Fortune 100
- Stores
- Orders
---
