---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: framelane.io
  spf: true
hosts:
- cert_expires: Jan  6 00:29:56 2027 GMT
  host: framelane.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Framelane Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for framelane-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: framelane-io
provider_slug: framelane-io
slug: framelane-io-domain-security
source_filename: framelane-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: framelane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 00:29:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: framelane.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/framelane-io/security/framelane-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video Editing
- Rendering API
- AI Agents
- GPU Rendering
- Video Production
- SDK
---
