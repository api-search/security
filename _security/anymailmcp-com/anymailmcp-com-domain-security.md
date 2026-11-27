---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: anymailmcp.com
  spf: true
hosts:
- cert_expires: Dec 10 20:40:22 2026 GMT
  host: anymailmcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: anymailmcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for anymailmcp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: anymailmcp
provider_slug: anymailmcp-com
slug: anymailmcp-com-domain-security
source_filename: anymailmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anymailmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 20:40:22 2026 GMT\n  hsts: false\ndomains:\n- domain: anymailmcp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anymailmcp-com/security/anymailmcp-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email
- MCP
- Artificial Intelligence
- Hosted
- IMAP
---
