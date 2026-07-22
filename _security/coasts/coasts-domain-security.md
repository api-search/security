---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coasts.dev
  spf: true
hosts:
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: coasts.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coasts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coasts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coasts
provider_slug: coasts
slug: coasts-domain-security
source_filename: coasts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coasts.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: coasts.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coasts/refs/heads/main/security/coasts-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Tools
- CLI
- Git
- Containers
- Docker
- Local Development
- AI Agents
- Developer Productivity
- Open Source
- DevOps
---
