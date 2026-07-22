---
api_specs:
- filename: parsec-teams-openapi.yml
  format: yaml
  label: Parsec for Teams API
  slug: parsec-for-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/openapi/parsec-teams-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parsec.app
  spf: true
hosts:
- cert_expires: Sep 15 04:04:51 2026 GMT
  host: api.parsec.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parsec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parsec
provider_slug: parsec
slug: parsec-domain-security
source_filename: parsec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.parsec.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:04:51 2026 GMT\n  hsts: null\ndomains:\n- domain: parsec.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsec/refs/heads/main/security/parsec-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Remote Desktop
- Cloud Gaming
- Streaming
- Virtual Desktop
- Team Management
- Developer Tools
- Gaming
---
