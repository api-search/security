---
api_specs:
- filename: stackexchange-api-v2-3.yaml
  format: yaml
  label: Stack Exchange API v2.3
  slug: stack-exchange-api-v23
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-api-v2-3.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackexchange.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: stackoverflowteams.help
  spf: true
hosts:
- cert_expires: Sep 16 06:02:09 2026 GMT
  host: stackexchange.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 22:33:35 2026 GMT
  host: api.stackexchange.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 19:16:28 2026 GMT
  host: stackoverflowteams.help
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stackexchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stack Exchange, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stack Exchange
provider_slug: stackexchange
slug: stackexchange-domain-security
source_filename: stackexchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stackexchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:02:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stackexchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:33:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: stackoverflowteams.help\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:16:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stackexchange.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stackoverflowteams.help\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/security/stackexchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Q And A
- Developer Community
- Knowledge Graph
- Stack Overflow
- Stack Exchange
- Reputation
- Tags
- Community
- MCP
- AI Grounding
---
