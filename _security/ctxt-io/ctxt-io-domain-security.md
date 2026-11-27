---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ctxt.io
  spf: false
hosts:
- cert_expires: Dec 13 15:09:02 2026 GMT
  host: ctxt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Context Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Context, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Context
provider_slug: ctxt-io
slug: ctxt-io-domain-security
source_filename: ctxt-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ctxt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 15:09:02 2026 GMT\n  hsts: false\ndomains:\n- domain: ctxt.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ctxt-io/security/ctxt-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Pastebin
- Content Sharing
- MCP
- AI Agents
- Browser Extension
- Developer Tools
---
