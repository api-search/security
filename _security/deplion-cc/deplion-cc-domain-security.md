---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deplion.cc
  spf: true
hosts:
- cert_expires: Dec 17 11:57:14 2026 GMT
  host: deplion.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deplion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deplion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deplion
provider_slug: deplion-cc
slug: deplion-cc-domain-security
source_filename: deplion-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deplion.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 11:57:14 2026 GMT\n  hsts: false\ndomains:\n- domain: deplion.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/deplion-cc/security/deplion-cc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- MCP
- Website Publishing
- Web Hosting
- Deployment
- No-Code
- AI Agents
---
