---
api_specs:
- filename: unleash-admin-api-openapi.yml
  format: yaml
  label: Unleash Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unleash/refs/heads/main/openapi/unleash-admin-api-openapi.yml
- filename: unleash-client-api-openapi.yml
  format: yaml
  label: Unleash Client API
  slug: client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unleash/refs/heads/main/openapi/unleash-client-api-openapi.yml
- filename: unleash-frontend-api-openapi.yml
  format: yaml
  label: Unleash Frontend API
  slug: frontend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unleash/refs/heads/main/openapi/unleash-frontend-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getunleash.io
  spf: true
hosts:
- cert_expires: Aug 12 19:51:13 2026 GMT
  host: www.getunleash.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 04:14:45 2026 GMT
  host: docs.getunleash.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unleash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unleash, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unleash
provider_slug: unleash
slug: unleash-domain-security
source_filename: unleash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getunleash.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 19:51:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.getunleash.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 04:14:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getunleash.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unleash/refs/heads/main/security/unleash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Feature Flags
- Feature Management
- Progressive Delivery
- A/B Testing
- Open Source
- Developer Tools
---
