---
api_specs:
- filename: zuora-v1-openapi.yml
  format: yaml
  label: Zuora V1 API
  slug: v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuora/refs/heads/main/openapi/zuora-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zuora.com
  spf: true
hosts:
- cert_expires: Sep 21 12:59:16 2026 GMT
  host: developer.zuora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.zuora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: rest.zuora.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zuora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zuora, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zuora
provider_slug: zuora
slug: zuora-domain-security
source_filename: zuora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.zuora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:59:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.zuora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.zuora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: zuora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuora/refs/heads/main/security/zuora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Finance
- Payments
- Subscriptions
---
