---
api_specs:
- filename: frejun-teler-events-api-openapi.yml
  format: yaml
  label: FreJun Teler Events API
  slug: frejun-teler-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-events-api-openapi.yml
- filename: frejun-teler-secrets-api-openapi.yml
  format: yaml
  label: FreJun Teler Secrets API
  slug: frejun-teler-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-secrets-api-openapi.yml
- filename: frejun-teler-sip-calls-api-openapi.yml
  format: yaml
  label: FreJun Teler SIP / Calls API
  slug: frejun-teler-sip-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-sip-calls-api-openapi.yml
- filename: frejun-teler-sip-ip-access-control-lists-api-openapi.yml
  format: yaml
  label: FreJun Teler SIP / IP Access Control Lists API
  slug: frejun-teler-sip-ip-access-control-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-sip-ip-access-control-lists-api-openapi.yml
- filename: frejun-teler-sip-trunks-api-openapi.yml
  format: yaml
  label: FreJun Teler SIP / Trunks API
  slug: frejun-teler-sip-trunks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-sip-trunks-api-openapi.yml
- filename: frejun-teler-utilities-api-openapi.yml
  format: yaml
  label: FreJun Teler Utilities API
  slug: frejun-teler-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-utilities-api-openapi.yml
- filename: frejun-teler-virtual-numbers-api-openapi.yml
  format: yaml
  label: FreJun Teler Virtual Numbers API
  slug: frejun-teler-virtual-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-virtual-numbers-api-openapi.yml
- filename: frejun-teler-voice-apps-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Apps API
  slug: frejun-teler-voice-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-apps-api-openapi.yml
- filename: frejun-teler-voice-call-controls-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Call Controls API
  slug: frejun-teler-voice-call-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-call-controls-api-openapi.yml
- filename: frejun-teler-voice-calls-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Calls API
  slug: frejun-teler-voice-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-calls-api-openapi.yml
- filename: frejun-teler-voice-calls-legacy-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Calls (legacy) API
  slug: frejun-teler-voice-calls-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-calls-legacy-api-openapi.yml
- filename: frejun-teler-voice-operations-api-openapi.yml
  format: yaml
  label: FreJun Teler Voice / Operations API
  slug: frejun-teler-voice-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/openapi/frejun-teler-voice-operations-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: frejun.ai
  spf: true
hosts:
- cert_expires: Dec 14 00:55:52 2026 GMT
  host: www.frejun.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 08:47:44 2026 GMT
  host: api.frejun.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Frejun Teler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreJun Teler, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FreJun Teler
provider_slug: frejun-teler
slug: frejun-teler-domain-security
source_filename: frejun-teler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.frejun.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 00:55:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.frejun.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 08:47:44 2026 GMT\n  hsts: null\ndomains:\n- domain: frejun.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frejun-teler/refs/heads/main/security/frejun-teler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- programmable voice API
- voice AI infrastructure
- CPaaS
- SIP Trunking
- telephony API
- real-time media streaming
- WebSocket audio
- Call Automation
- conversational AI infrastructure
---
