---
api_specs:
- filename: arcjet-openapi.yml
  format: yaml
  label: Arcjet Decide API
  slug: arcjet-decide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/openapi/arcjet-openapi.yml
- filename: arcjet-openapi.yml
  format: yaml
  label: Arcjet Rate Limiting
  slug: arcjet-rate-limiting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/openapi/arcjet-openapi.yml
- filename: arcjet-openapi.yml
  format: yaml
  label: Arcjet Bot Detection
  slug: arcjet-bot-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/openapi/arcjet-openapi.yml
- filename: arcjet-openapi.yml
  format: yaml
  label: Arcjet Email Validation
  slug: arcjet-email-validation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/openapi/arcjet-openapi.yml
- filename: arcjet-openapi.yml
  format: yaml
  label: Arcjet Sensitive Information Detection
  slug: arcjet-sensitive-info-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/openapi/arcjet-openapi.yml
- filename: arcjet-openapi.yml
  format: yaml
  label: Arcjet Shield WAF
  slug: arcjet-shield-waf
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/openapi/arcjet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arcjet.com
  spf: true
hosts:
- cert_expires: Sep 18 06:34:23 2026 GMT
  host: arcjet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 07:26:18 2026 GMT
  host: docs.arcjet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: decide.arcjet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arcjet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcjet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arcjet
provider_slug: arcjet
slug: arcjet-domain-security
source_filename: arcjet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 06:34:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.arcjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:26:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: decide.arcjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: arcjet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/security/arcjet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Rate Limiting
- Bot Detection
- WAF
- Developer Security
---
