---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentreputation.dev
  spf: false
hosts:
- cert_expires: Dec 18 17:20:09 2026 GMT
  host: agentreputation.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentreputation Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Reputation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agent Reputation
provider_slug: agentreputation-dev
slug: agentreputation-dev-domain-security
source_filename: agentreputation-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentreputation.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 17:20:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentreputation.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentreputation-dev/security/agentreputation-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Evidence
- Complaint
- Marketplace
- Platform
- Company
---
