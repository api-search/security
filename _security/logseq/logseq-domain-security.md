---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: logseq.com
  spf: false
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: logseq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logseq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logseq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Logseq
provider_slug: logseq
slug: logseq-domain-security
source_filename: logseq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logseq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: logseq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logseq/refs/heads/main/security/logseq-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Knowledge Management
- Note Taking
- Productivity
- Open Source
- Plugins
- SDK
- Knowledge Graph
- Markdown
- Local-First
- Developer Tools
---
