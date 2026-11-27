---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: commentify.one
  spf: true
hosts:
- cert_expires: Dec 21 12:14:12 2026 GMT
  host: commentify.one
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Commentify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commentify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Commentify
provider_slug: commentify-one
slug: commentify-one-domain-security
source_filename: commentify-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commentify.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 12:14:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: commentify.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/commentify-one/security/commentify-one-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Feedback
- Design Collaboration
- Comments
- MCP
- AI Agents
- Figma
- Jira
- Notion
---
