---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: melaya.org
  spf: true
hosts:
- cert_expires: Feb 14 16:29:33 2027 GMT
  host: melaya.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Melaya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Melaya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Melaya
provider_slug: melaya-org
slug: melaya-org-domain-security
source_filename: melaya-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: melaya.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 16:29:33 2027 GMT\n  hsts: null\ndomains:\n- domain: melaya.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/melaya-org/security/melaya-org-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Agents
- Platform
- Automation
- MCP
---
