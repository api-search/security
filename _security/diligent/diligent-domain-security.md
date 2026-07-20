---
api_specs:
- filename: diligent-openapi-original.json
  format: json
  label: Diligent API
  slug: diligent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-openapi-original.json
- filename: diligent-remediation-openapi.json
  format: json
  label: Diligent Remediation API (Beta)
  slug: diligent-remediation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-remediation-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: godiligent.ai
  spf: true
hosts:
- cert_expires: Sep 28 12:39:28 2026 GMT
  host: www.godiligent.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 18:42:40 2026 GMT
  host: docs.godiligent.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: api.godiligent.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diligent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diligent, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diligent
provider_slug: diligent
slug: diligent-domain-security
source_filename: diligent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.godiligent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:39:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.godiligent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:42:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.godiligent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: godiligent.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/security/diligent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- RegTech
- KYC
- AML
- Financial Crime
- Due Diligence
- Screening
- Sanctions
- Monitoring
- Artificial Intelligence
- Fintech
- Webhooks
---
