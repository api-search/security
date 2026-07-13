---
api_specs:
- filename: vapi-openapi.yml
  format: yaml
  label: Vapi Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi/refs/heads/main/openapi/vapi-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vapi.ai
  spf: true
hosts:
- cert_expires: Sep 30 05:31:31 2026 GMT
  host: vapi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 14:20:51 2026 GMT
  host: docs.vapi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 06:52:46 2026 GMT
  host: api.vapi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vapi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vapi
provider_slug: vapi
slug: vapi-domain-security
source_filename: vapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:31:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.vapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 14:20:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:52:46 2026 GMT\n  hsts: false\ndomains:\n- domain: vapi.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vapi/refs/heads/main/security/vapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Voice
- Agents
- Realtime
- CPaaS
---
