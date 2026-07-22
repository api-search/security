---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stagereview.app
  spf: true
hosts:
- cert_expires: Sep 26 21:56:16 2026 GMT
  host: stagereview.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stage
provider_slug: stage
slug: stage-domain-security
source_filename: stage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stagereview.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 21:56:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stagereview.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stage/refs/heads/main/security/stage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Code Review
- Developer Tools
- CLI
- AI Coding Agents
- Pull Requests
- Git
- Software Development
---
