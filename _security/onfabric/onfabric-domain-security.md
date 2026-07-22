---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: onfabric.io
  spf: true
hosts:
- cert_expires: Sep 30 09:37:53 2026 GMT
  host: onfabric.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onfabric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OnFabric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OnFabric
provider_slug: onfabric
slug: onfabric-domain-security
source_filename: onfabric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onfabric.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:37:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: onfabric.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onfabric/refs/heads/main/security/onfabric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- AI Agents
- Personal Context
- Memory
- Model Context Protocol
- Developer Tools
- CLI
---
