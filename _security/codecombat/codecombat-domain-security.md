---
api_specs:
- filename: codecombat-openapi-original.yml
  format: yaml
  label: CodeCombat Partner API
  slug: codecombat-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/openapi/codecombat-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codecombat.com
  spf: true
hosts:
- cert_expires: Oct  3 11:26:25 2026 GMT
  host: api-docs.codecombat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 11:26:25 2026 GMT
  host: codecombat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codecombat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeCombat, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CodeCombat
provider_slug: codecombat
slug: codecombat-domain-security
source_filename: codecombat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-docs.codecombat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:26:25 2026 GMT\n  hsts: false\n- host: codecombat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:26:25 2026 GMT\n  hsts: false\ndomains:\n- domain: codecombat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/security/codecombat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Coding
- Learning
- Classroom
- Students
- Gamification
- SSO
- Developer Tools
---
