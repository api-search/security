---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: codemindhq.dev
  spf: true
hosts:
- cert_expires: Jan 23 05:42:35 2027 GMT
  host: codemindhq.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CodeMind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeMind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CodeMind
provider_slug: codemindhq-dev
slug: codemindhq-dev-domain-security
source_filename: codemindhq-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codemindhq.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 05:42:35 2027 GMT\n  hsts: false\ndomains:\n- domain: codemindhq.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/codemindhq-dev/security/codemindhq-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI Coding
- Code Generation
- MCP
- Developer Tools
- GitHub
- Pull Requests
- Code Verification
---
