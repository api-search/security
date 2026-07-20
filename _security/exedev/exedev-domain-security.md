---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exe.dev
  spf: false
hosts:
- cert_expires: Aug 20 17:21:07 2026 GMT
  host: exe.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exedev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for exe.dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: exe.dev
provider_slug: exedev
slug: exedev-domain-security
source_filename: exedev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exe.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: exe.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exedev/refs/heads/main/security/exedev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Cloud Computing
- Virtual Machines
- Sandbox
- AI Agents
- Infrastructure
- SSH
---
