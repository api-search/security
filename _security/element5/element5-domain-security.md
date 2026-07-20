---
api_specs:
- filename: element5-openapi-original.json
  format: json
  label: Element5 API
  slug: element5-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element5/refs/heads/main/openapi/element5-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: e5.ai
  spf: true
hosts:
- cert_expires: Oct  6 18:53:43 2026 GMT
  host: www.e5.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api-doc.e5.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.e5.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Element5 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Element5, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Element5
provider_slug: element5
slug: element5-domain-security
source_filename: element5-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.e5.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 18:53:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-doc.e5.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: api.e5.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: e5.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/element5/refs/heads/main/security/element5-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Post-Acute Care
- Workflow Automation
- Eligibility Verification
- Prior Authorization
- Claims Processing
- Webhooks
- Artificial Intelligence
---
