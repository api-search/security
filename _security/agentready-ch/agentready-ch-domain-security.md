---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: agentready.ch
  spf: true
hosts:
- cert_expires: Jan  2 14:00:30 2027 GMT
  host: agentready.ch
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentready Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent-ready, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Agent-ready
provider_slug: agentready-ch
slug: agentready-ch-domain-security
source_filename: agentready-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentready.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 14:00:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentready.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentready-ch/security/agentready-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Directory
- Artificial Intelligence
- Switzerland
- Software-as-a-Service
---
