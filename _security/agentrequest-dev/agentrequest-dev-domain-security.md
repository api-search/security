---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: agentrequest.dev
  spf: false
hosts:
- cert_expires: Jan 15 00:23:42 2027 GMT
  host: agentrequest.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Request Desk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Request Desk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agent Request Desk
provider_slug: agentrequest-dev
slug: agentrequest-dev-domain-security
source_filename: agentrequest-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentrequest.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 00:23:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentrequest.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentrequest-dev/security/agentrequest-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- MCP
- Diagnostics
- Free
- United Kingdom
---
