---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dev.fast
  spf: true
hosts:
- cert_expires: Oct  2 17:14:47 2026 GMT
  host: dev.fast
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devfast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for /dev/fast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: /dev/fast
provider_slug: devfast
slug: devfast-domain-security
source_filename: devfast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.fast\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:14:47 2026 GMT\n  hsts: false\ndomains:\n- domain: dev.fast\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devfast/refs/heads/main/security/devfast-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Developer Tools
- Code Review
- Code Hosting
- Deployment
- CI/CD
- AI Agents
- Y Combinator
---
