---
api_specs:
- filename: _doc
  format: yaml
  label: Penpot RPC API
  slug: penpot-rpc-api
  spec_type: OpenAPI
  url: https://design.penpot.app/api/_doc
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: penpot.app
  spf: true
hosts:
- cert_expires: Aug 19 10:56:28 2026 GMT
  host: penpot.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 16:27:55 2026 GMT
  host: design.penpot.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 17:56:14 2026 GMT
  host: help.penpot.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Penpot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Penpot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Penpot
provider_slug: penpot
slug: penpot-domain-security
source_filename: penpot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: penpot.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:56:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: design.penpot.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:27:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: help.penpot.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:56:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: penpot.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/penpot/refs/heads/main/security/penpot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Prototyping
- Open Source
- Self-Hosted
- Figma Alternative
- UI Design
- Collaboration
- Design Systems
---
