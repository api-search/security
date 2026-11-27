---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buy-my-agent.com
  spf: true
hosts:
- cert_expires: Jan 19 21:43:25 2027 GMT
  host: buy-my-agent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buy My Agent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buy My Agent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Buy My Agent
provider_slug: buy-my-agent-com
slug: buy-my-agent-com-domain-security
source_filename: buy-my-agent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buy-my-agent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 21:43:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buy-my-agent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/buy-my-agent-com/security/buy-my-agent-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Marketplace
- Automation
- Agents
- Business
---
