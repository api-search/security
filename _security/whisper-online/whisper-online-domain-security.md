---
api_specs:
- filename: whisper-online-openapi.json
  format: json
  label: Whisper API
  slug: whisper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: whisper.online
  spf: true
hosts:
- cert_expires: Dec 18 20:13:49 2026 GMT
  host: whisper.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Whisper Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whisper Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Whisper Security
provider_slug: whisper-online
slug: whisper-online-domain-security
source_filename: whisper-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whisper.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 20:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whisper.online\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/security/whisper-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agent Identity
- Agents
- IPv6
- DNS
- DNSSEC
- Threat Intelligence
- Security
- Egress
- A2A
- MCP
- RDAP
- Transparency Log
- Graph Database
- agent-native
- Netherlands
---
