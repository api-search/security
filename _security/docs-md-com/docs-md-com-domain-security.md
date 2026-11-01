---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: docs-md.com
  spf: false
hosts:
- cert_expires: Nov 28 00:35:42 2026 GMT
  host: docs-md.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docs Md Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for docs-md-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: docs-md-com
provider_slug: docs-md-com
slug: docs-md-com-domain-security
source_filename: docs-md-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs-md.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 00:35:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: docs-md.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/docs-md-com/security/docs-md-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Markdown
- AI
- MCP
- Sharing
- Free
---
