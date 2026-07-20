---
api_specs:
- filename: earnipay-e-invoicing-openapi-original.json
  format: json
  label: Earnipay Invoicing API
  slug: earnipay-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-e-invoicing-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: earnipay.com
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: earnipay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:40:17 2026 GMT
  host: docs.earnipay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 20:15:15 2026 GMT
  host: e-invoicing.earnipay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earnipay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earnipay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Earnipay
provider_slug: earnipay
slug: earnipay-domain-security
source_filename: earnipay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earnipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\n- host: docs.earnipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: e-invoicing.earnipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:15:15 2026 GMT\n  hsts: null\ndomains:\n- domain: earnipay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/security/earnipay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Invoicing
- Invoicing
- FIRS
- NRS
- Tax
- Compliance
- Fintech
- Nigeria
- Payments
- Financial Services
---
