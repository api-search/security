---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentsql.cn
  spf: false
hosts:
- cert_expires: Dec 29 03:24:06 2026 GMT
  host: agentsql.cn
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentsql Cn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentSQL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentSQL
provider_slug: agentsql-cn
slug: agentsql-cn-domain-security
source_filename: agentsql-cn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentsql.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 03:24:06 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: agentsql.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentsql-cn/security/agentsql-cn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Database
- Security
- Artificial Intelligence
- Open Source
- Gateways
---
