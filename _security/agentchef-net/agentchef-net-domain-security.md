---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentchef.net
  spf: true
hosts:
- cert_expires: Dec  4 19:08:15 2026 GMT
  host: agentchef.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Chef Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Chef, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agent Chef
provider_slug: agentchef-net
slug: agentchef-net-domain-security
source_filename: agentchef-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentchef.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 19:08:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentchef.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentchef-net/security/agentchef-net-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Dinner Planning
- Family
- Meal Service
---
