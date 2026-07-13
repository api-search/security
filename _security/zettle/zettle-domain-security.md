---
api_specs:
- filename: zettle-finance-api-openapi.yaml
  format: yaml
  label: Zettle Finance API
  slug: zettle-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zettle/refs/heads/main/openapi/zettle-finance-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zettle.com
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: www.zettle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: developer.zettle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: oauth.zettle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zettle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zettle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zettle
provider_slug: zettle
slug: zettle-domain-security
source_filename: zettle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zettle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.zettle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: oauth.zettle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zettle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zettle/refs/heads/main/security/zettle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Point of Sale
- POS
- Payments
- Inventory
- Finance
- PayPal
- Card Payments
- Merchant Services
---
