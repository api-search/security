---
api_specs:
- filename: getemboss-ai-account-openapi.yml
  format: yaml
  label: Emboss Account API
  slug: emboss-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/openapi/getemboss-ai-account-openapi.yml
- filename: getemboss-ai-pay-per-call-openapi.yml
  format: yaml
  label: Emboss Pay-per-call API
  slug: emboss-pay-per-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/openapi/getemboss-ai-pay-per-call-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getemboss.ai
  spf: false
hosts:
- cert_expires: Nov  2 19:51:33 2026 GMT
  host: getemboss.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 16:53:41 2026 GMT
  host: api.getemboss.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Getemboss Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emboss, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Emboss
provider_slug: getemboss-ai
slug: getemboss-ai-domain-security
source_filename: getemboss-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getemboss.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:51:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.getemboss.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 16:53:41 2026 GMT\n  hsts: null\ndomains:\n- domain: getemboss.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getemboss-ai/refs/heads/main/security/getemboss-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Forms
- Document Processing
- Form Filling
- Fax
- Data Extraction
- agent-native
- MCP
- A2A
- x402
- pay-per-call
- Government Forms
- Company
---
