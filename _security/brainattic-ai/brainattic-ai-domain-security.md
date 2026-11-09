---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: brainattic.ai
  spf: true
hosts:
- cert_expires: Jan 27 07:42:00 2027 GMT
  host: brainattic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainattic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for brainattic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: brainattic
provider_slug: brainattic-ai
slug: brainattic-ai-domain-security
source_filename: brainattic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brainattic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 07:42:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brainattic.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/brainattic-ai/security/brainattic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Knowledge Base
- Artificial Intelligence
- Enterprise
- Governance
- MCP
- Company
---
