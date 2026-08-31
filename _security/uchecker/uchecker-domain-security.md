---
api_specs:
- filename: uchecker-default-api-openapi.yml
  format: yaml
  label: uChecker Аутентификация API
  slug: uchecker-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uchecker/refs/heads/main/openapi/uchecker-default-api-openapi.yml
- filename: uchecker-email-api-openapi.yml
  format: yaml
  label: uChecker Валидация Email API
  slug: uchecker-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uchecker/refs/heads/main/openapi/uchecker-email-api-openapi.yml
- filename: uchecker-esp-api-openapi.yml
  format: yaml
  label: uChecker ESP Провайдеры API
  slug: uchecker-esp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uchecker/refs/heads/main/openapi/uchecker-esp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uchecker.net
  spf: true
hosts:
- cert_expires: Sep 18 16:29:18 2026 GMT
  host: api.uchecker.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uchecker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for uChecker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: uChecker
provider_slug: uchecker
slug: uchecker-domain-security
source_filename: uchecker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.uchecker.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:29:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uchecker.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uchecker/refs/heads/main/security/uchecker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- email-verification
- Email
- SMTP
- dns
- deliverability
- mx
- spf
- dkim
- DMARC
- MCP
- agent-native
- data-quality
---
