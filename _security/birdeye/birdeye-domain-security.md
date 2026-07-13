---
api_specs:
- filename: birdeye-birdeye-api-openapi.yml
  format: yaml
  label: Birdeye API
  slug: birdeye-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/birdeye/refs/heads/main/openapi/birdeye-birdeye-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: birdeye.com
  spf: true
hosts:
- cert_expires: Oct 19 13:18:47 2026 GMT
  host: birdeye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 13:18:47 2026 GMT
  host: developers.birdeye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 13:18:47 2026 GMT
  host: api.birdeye.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Birdeye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Birdeye, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Birdeye
provider_slug: birdeye
slug: birdeye-domain-security
source_filename: birdeye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: birdeye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 13:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.birdeye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 13:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.birdeye.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 13:18:47 2026 GMT\n  hsts: null\ndomains:\n- domain: birdeye.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/birdeye/refs/heads/main/security/birdeye-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Reputation Management
- Reviews
- Customer Experience
- Surveys
- Messaging
- Multi-Location
- AI
---
