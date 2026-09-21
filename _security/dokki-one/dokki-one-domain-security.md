---
api_specs:
- filename: dokki-one-openapi.yml
  format: yaml
  label: Dokki API
  slug: dokki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dokki-one/refs/heads/main/openapi/dokki-one-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dokki.one
  spf: false
hosts:
- cert_expires: Oct 20 18:42:25 2026 GMT
  host: dokki.one
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dokki One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dokki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Dokki
provider_slug: dokki-one
slug: dokki-one-domain-security
source_filename: dokki-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dokki.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 18:42:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dokki.one\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dokki-one/refs/heads/main/security/dokki-one-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Knowledge-Management
- Documents
- Agents
- MCP
- Artificial Intelligence
- Productivity
- Workspace
- Publishing
- Search
- Singapore
---
