---
api_specs:
- filename: localxpose-openapi-generated.yml
  format: yaml
  label: xLab API
  slug: localxpose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localxpose/refs/heads/main/openapi/_ae-authored/localxpose-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: localxpose.io
  spf: true
hosts:
- cert_expires: Nov 18 13:50:10 2026 GMT
  host: localxpose.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Localxpose Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: xLab
provider_slug: localxpose
slug: localxpose-domain-security
source_filename: localxpose-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localxpose.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 13:50:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: localxpose.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localxpose/refs/heads/main/security/localxpose-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tunneling
- Developer Tools
- Security
- Cloud
- Networking
---
