---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: digger.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opencomputer.dev
  spf: true
hosts:
- cert_expires: Oct  5 18:42:27 2026 GMT
  host: digger.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:41:07 2026 GMT
  host: docs.opencomputer.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 03:25:18 2026 GMT
  host: app.opencomputer.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digger, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Digger
provider_slug: digger
slug: digger-domain-security
source_filename: digger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digger.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.opencomputer.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:41:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.opencomputer.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 03:25:18 2026 GMT\n  hsts: false\ndomains:\n- domain: digger.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: opencomputer.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digger/refs/heads/main/security/digger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Cloud Sandbox
- Compute
- Infrastructure as Code
- Terraform
- OpenTofu
- Developer Tools
- Webhooks
- Open Source
- SDKs
- CLI
---
