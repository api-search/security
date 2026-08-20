---
api_specs:
- filename: feedly-streams-openapi.yml
  format: yaml
  label: Feedly API
  slug: feedly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feedly/refs/heads/main/openapi/feedly-streams-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: feedly.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: feedly.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 11:26:20 2026 GMT
  host: developers.feedly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.feedly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Feedly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feedly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Feedly
provider_slug: feedly
slug: feedly-domain-security
source_filename: feedly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: feedly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.feedly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:26:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.feedly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: feedly.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feedly/refs/heads/main/security/feedly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Threat Intelligence
- Cybersecurity
- cyber-threat-intelligence
- Content Aggregation
- RSS
- News
- Vulnerability Management
- Indicators of Compromise
- Malware
- threat-actors
- mitre-attack
- Security Automation
- Artificial Intelligence
- MCP
- agent-native
- Webhook
---
