---
api_specs:
- filename: obsidian-local-rest-api-openapi.yaml
  format: yaml
  label: Obsidian Local REST API
  slug: obsidian-local-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-local-rest-api-openapi.yaml
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
  domain: obsidian.md
  spf: true
hosts:
- cert_expires: Aug 28 12:19:07 2026 GMT
  host: obsidian.md
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 12:19:07 2026 GMT
  host: docs.obsidian.md
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Obsidian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obsidian, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Obsidian
provider_slug: obsidian
slug: obsidian-domain-security
source_filename: obsidian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obsidian.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:19:07 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: docs.obsidian.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:19:07 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: obsidian.md\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/security/obsidian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Knowledge Management
- Markdown
- Notes
- Local-First
---
