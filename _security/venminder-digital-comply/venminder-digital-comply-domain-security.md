---
api_specs:
- filename: venminder-digital-comply-openapi-original.json
  format: json
  label: Venminder API
  slug: venminder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venminder-digital-comply/refs/heads/main/openapi/venminder-digital-comply-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: venminder.com
  spf: true
hosts:
- cert_expires: Oct 19 11:31:47 2026 GMT
  host: www.venminder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 16:20:12 2026 GMT
  host: developers.venminder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 20:42:38 2027 GMT
  host: rsd.venminder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Venminder Digital Comply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Venminder (Digital Comply), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Venminder (Digital Comply)
provider_slug: venminder-digital-comply
slug: venminder-digital-comply-domain-security
source_filename: venminder-digital-comply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.venminder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 11:31:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.venminder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:20:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rsd.venminder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 20:42:38 2027 GMT\n  hsts: null\ndomains:\n- domain: venminder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venminder-digital-comply/refs/heads/main/security/venminder-digital-comply-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Third-Party Risk Management
- Vendor Management
- Risk
- Compliance
- Contracts
- Financial Services
- Due Diligence
- SCIM
---
