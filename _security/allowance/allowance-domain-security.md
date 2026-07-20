---
api_specs:
- filename: allowance-openapi-original.json
  format: json
  label: Allowance API
  slug: allowance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allowance/refs/heads/main/openapi/allowance-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useallowance.com
  spf: true
hosts:
- cert_expires: Oct  3 02:23:15 2026 GMT
  host: useallowance.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:34:23 2026 GMT
  host: api.useallowance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allowance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allowance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Allowance
provider_slug: allowance
slug: allowance-domain-security
source_filename: allowance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useallowance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:23:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.useallowance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:34:23 2026 GMT\n  hsts: null\ndomains:\n- domain: useallowance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allowance/refs/heads/main/security/allowance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Agentic Payments
- AI Agents
- Virtual Cards
- Fintech
- Model Context Protocol
- Consumer Trust
- Spending Controls
- AP2
---
