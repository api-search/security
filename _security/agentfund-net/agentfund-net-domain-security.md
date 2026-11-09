---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentfund.net
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: agentfund.net
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentfund Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Fund Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agent Fund Ventures
provider_slug: agentfund-net
slug: agentfund-net-domain-security
source_filename: agentfund-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentfund.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: agentfund.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentfund-net/security/agentfund-net-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Venture Capital
- Funding
- Autonomous-Economy
- Startups
---
