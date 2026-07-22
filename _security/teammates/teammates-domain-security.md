---
api_specs:
- filename: teammates-smarttools-openapi.yaml
  format: yaml
  label: Teammates SmartTools API
  slug: teammates-smarttools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teammates/refs/heads/main/openapi/teammates-smarttools-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: teammates.work
  spf: true
hosts:
- cert_expires: Sep 30 13:30:32 2026 GMT
  host: teammates.work
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.teammates.work
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.teammat'
kind: domain-security
layout: security
method: probed
name: Teammates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teammates, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Teammates
provider_slug: teammates
slug: teammates-domain-security
source_filename: teammates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teammates.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:30:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.teammates.work\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.teammat'\n  hsts: null\ndomains:\n- domain: teammates.work\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teammates/refs/heads/main/security/teammates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- B2B
- Artificial Intelligence
- AI Agents
- Virtual Workforce
- Automation
- Productivity
- SaaS
- MCP
---
