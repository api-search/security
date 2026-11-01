---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: strandsagents.com
  spf: false
hosts:
- cert_expires: Dec  8 05:43:21 2026 GMT
  host: strandsagents.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Strandsagents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strands Agents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Strands Agents
provider_slug: strandsagents
slug: strandsagents-domain-security
source_filename: strandsagents-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strandsagents.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 05:43:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: strandsagents.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/strandsagents/security/strandsagents-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- OpenSource
- Toolkit
- Agents
---
