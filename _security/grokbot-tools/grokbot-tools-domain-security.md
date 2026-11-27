---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: grokbot.tools
  spf: false
hosts:
- cert_expires: Jan 16 02:51:19 2027 GMT
  host: grokbot.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: grokbot.tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for grokbot.tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: grokbot.tools
provider_slug: grokbot-tools
slug: grokbot-tools-domain-security
source_filename: grokbot-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grokbot.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 02:51:19 2027 GMT\n  hsts: false\ndomains:\n- domain: grokbot.tools\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/grokbot-tools/security/grokbot-tools-domain-security.yml
summary_line: TLSv1.3
tags:
- Directory
- MCP
- Connectors
- Open Source
- Community
---
