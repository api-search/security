---
api_specs:
- filename: textmaster-api-v1-openapi.yml
  format: yaml
  label: TextMaster API v1
  slug: textmaster-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-api-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: textmaster.com
  spf: true
hosts:
- cert_expires: Nov  9 10:41:14 2026 GMT
  host: www.textmaster.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 08:57:51 2026 GMT
  host: developer.textmaster.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 10:41:14 2026 GMT
  host: api.textmaster.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Textmaster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TextMaster, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TextMaster
provider_slug: textmaster
slug: textmaster-domain-security
source_filename: textmaster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.textmaster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 10:41:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.textmaster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 08:57:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.textmaster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 10:41:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: textmaster.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/security/textmaster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Translation
- Localization
- Language Services
- Copywriting
- Proofreading
- Machine Translation
- Content Production
- Translation Memory
- Glossary
- Ecommerce Localization
- Product Information Management
- Webhooks
- OAuth2
- SaaS
---
