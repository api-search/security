---
api_specs:
- filename: manageprompt-actions-api-openapi.yml
  format: yaml
  label: ManagePrompt Actions API
  slug: manageprompt-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manageprompt/refs/heads/main/openapi/manageprompt-actions-api-openapi.yml
- filename: manageprompt-sessions-api-openapi.yml
  format: yaml
  label: ManagePrompt Sessions API
  slug: manageprompt-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manageprompt/refs/heads/main/openapi/manageprompt-sessions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: manageprompt.com
  spf: false
hosts:
- cert_expires: Dec 10 03:57:21 2026 GMT
  host: manageprompt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Manageprompt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ManagePrompt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ManagePrompt
provider_slug: manageprompt
slug: manageprompt-domain-security
source_filename: manageprompt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manageprompt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 03:57:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: manageprompt.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manageprompt/refs/heads/main/security/manageprompt-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- LLM
- Debugging
- OpenSource
- DeveloperTools
---
