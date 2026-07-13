---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: taiga.io
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: taiga.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:20:45 2026 GMT
  host: docs.taiga.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: api.taiga.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taiga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taiga, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Taiga
provider_slug: taiga
slug: taiga-domain-security
source_filename: taiga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taiga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.taiga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:20:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.taiga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: taiga.io\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taiga/refs/heads/main/security/taiga-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agile
- Project Management
- Scrum
- Kanban
- Issue Tracking
- Open Source
- Sprints
- User Stories
- Epics
- Tasks
---
