---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qname.ai
  spf: true
hosts:
- cert_expires: Dec  6 17:03:44 2026 GMT
  host: qname.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qname Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QName AI WHOIS API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QName AI WHOIS API
provider_slug: qname
slug: qname-domain-security
source_filename: qname-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qname.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 17:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qname.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qname/refs/heads/main/security/qname-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- WHOIS
- RDAP
- domain-research
- Domain Search
- batch-lookup
- CLI
- Agent Tooling
- Agent Skills
- llms-txt
- Developer Tools
- Domain Intelligence
---
