---
api_specs:
- filename: qodo-openapi.yml
  format: yaml
  label: Qodo Merge (PR-Agent)
  slug: qodo-merge-pr-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo/refs/heads/main/openapi/qodo-openapi.yml
- filename: qodo-openapi.yml
  format: yaml
  label: Qodo Hosted API
  slug: qodo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo/refs/heads/main/openapi/qodo-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qodo.ai
  spf: true
hosts:
- cert_expires: Sep 20 12:49:18 2026 GMT
  host: www.qodo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 15:24:17 2026 GMT
  host: qodo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:24:58 2026 GMT
  host: docs.qodo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qodo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qodo
provider_slug: qodo
slug: qodo-domain-security
source_filename: qodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qodo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:49:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: qodo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:24:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.qodo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:24:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qodo.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qodo/refs/heads/main/security/qodo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Code Review
- Code Integrity
- Developer Tools
- Pull Requests
---
