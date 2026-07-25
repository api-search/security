---
api_specs:
- filename: gray-swan-activity-api-openapi.yml
  format: yaml
  label: Gray Swan Activity API
  slug: gray-swan-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gray-swan/refs/heads/main/openapi/gray-swan-activity-api-openapi.yml
- filename: gray-swan-cygnal-api-openapi.yml
  format: yaml
  label: Gray Swan Cygnal API
  slug: gray-swan-cygnal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gray-swan/refs/heads/main/openapi/gray-swan-cygnal-api-openapi.yml
- filename: gray-swan-policies-api-openapi.yml
  format: yaml
  label: Gray Swan Policies API
  slug: gray-swan-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gray-swan/refs/heads/main/openapi/gray-swan-policies-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: grayswan.ai
  spf: true
hosts:
- cert_expires: Sep  1 09:47:37 2026 GMT
  host: www.grayswan.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gray Swan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gray Swan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gray Swan
provider_slug: gray-swan
slug: gray-swan-domain-security
source_filename: gray-swan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.grayswan.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 09:47:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grayswan.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gray-swan/refs/heads/main/security/gray-swan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- AI Security
- LLM Security
- Guardrails
- Red Teaming
- AI Governance
- Prompt Injection
- Model Safety
- API Security
---
