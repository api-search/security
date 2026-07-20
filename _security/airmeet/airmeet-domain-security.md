---
api_specs:
- filename: airmeet-openapi.yml
  format: yaml
  label: Airmeet Public API
  slug: airmeet-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airmeet/refs/heads/main/openapi/airmeet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: airmeet.com
  spf: true
hosts:
- cert_expires: Oct  7 15:01:56 2026 GMT
  host: www.airmeet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 15:01:56 2026 GMT
  host: api-gateway.airmeet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 04:43:41 2026 GMT
  host: api-gateway-prod.eu.airmeet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airmeet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airmeet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Airmeet
provider_slug: airmeet
slug: airmeet-domain-security
source_filename: airmeet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airmeet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:01:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-gateway.airmeet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:01:56 2026 GMT\n  hsts: null\n- host: api-gateway-prod.eu.airmeet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 04:43:41 2026 GMT\n  hsts: null\ndomains:\n- domain: airmeet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airmeet/refs/heads/main/security/airmeet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cloud Saas
- Events
- Virtual Events
- Webinars
- Event Management
- Community
- Webhooks
---
