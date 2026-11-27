---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: get4agent.com
  spf: true
hosts:
- cert_expires: Jan 21 20:59:11 2027 GMT
  host: get4agent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GET4AGENT Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GET4AGENT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GET4AGENT
provider_slug: get4agent-com
slug: get4agent-com-domain-security
source_filename: get4agent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: get4agent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:59:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: get4agent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/get4agent-com/security/get4agent-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Marketplace
- Trust
- Agents
- Commerce
- Company
---
