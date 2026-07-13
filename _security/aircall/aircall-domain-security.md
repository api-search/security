---
api_specs:
- filename: aircall-webhooks-asyncapi.yml
  format: yaml
  label: Aircall Webhooks API
  slug: aircall-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/aircall/refs/heads/main/asyncapi/aircall-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aircall.io
  spf: true
hosts:
- cert_expires: Sep 18 16:56:01 2026 GMT
  host: aircall.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: developer.aircall.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: api.aircall.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aircall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aircall, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aircall
provider_slug: aircall
slug: aircall-domain-security
source_filename: aircall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aircall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.aircall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: api.aircall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aircall.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircall/refs/heads/main/security/aircall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- Voice
- Cloud Phone
- CRM
- Sales
---
