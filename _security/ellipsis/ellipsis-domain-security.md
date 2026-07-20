---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ellipsis.dev
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: app.ellipsis.dev
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.ellipsis.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.ellipsis.dev
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ellipsis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ellipsis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ellipsis
provider_slug: ellipsis
slug: ellipsis-domain-security
source_filename: ellipsis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.ellipsis.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\n- host: www.ellipsis.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\n- host: api.ellipsis.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ellipsis.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellipsis/refs/heads/main/security/ellipsis-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Code Review
- AI Agents
- Coding Agents
- Developer Tools
- Software Development
- Automation
- DevOps
- Pull Requests
---
