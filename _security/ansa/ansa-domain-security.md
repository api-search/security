---
api_specs:
- filename: ansa-openapi-original.yml
  format: yaml
  label: Ansa API
  slug: ansa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/openapi/ansa-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ansa.dev
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getansa.com
  spf: true
hosts:
- cert_expires: Aug 16 14:12:43 2026 GMT
  host: www.ansa.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.getansa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api-sandbox.getansa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ansa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansa, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ansa
provider_slug: ansa
slug: ansa-domain-security
source_filename: ansa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ansa.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:12:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getansa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\n- host: api-sandbox.getansa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ansa.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getansa.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/security/ansa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Stored Value
- Digital Wallet
- Loyalty
- Incentives
- API
---
