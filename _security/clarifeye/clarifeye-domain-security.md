---
api_specs:
- filename: clarifeye-openapi-original.yaml
  format: yaml
  label: Clarifeye Platform API — Public
  slug: clarifeye-platform-api-public
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-openapi-original.yaml
- filename: clarifeye-backoffice-openapi-original.yaml
  format: yaml
  label: Clarifeye Platform API — Backoffice
  slug: clarifeye-platform-api-backoffice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-backoffice-openapi-original.yaml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clarifeye.ai
  spf: true
hosts:
- cert_expires: Sep  8 17:34:25 2026 GMT
  host: www.clarifeye.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 09:08:27 2026 GMT
  host: eu.app.clarifeye.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 11:49:12 2026 GMT
  host: us.app.clarifeye.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clarifeye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clarifeye, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clarifeye
provider_slug: clarifeye
slug: clarifeye-domain-security
source_filename: clarifeye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clarifeye.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:34:25 2026 GMT\n  hsts: false\n- host: eu.app.clarifeye.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:08:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.app.clarifeye.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:49:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clarifeye.ai\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/security/clarifeye-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Knowledge Management
- Model Context Protocol
- Document Intelligence
- Agents
- Enterprise AI
- Retrieval
---
