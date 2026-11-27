---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    agents: []
    checked: '2026-11-25'
    index:
    - alpn:
      - mcp
      target: mcp.symvanta.com
    published: true
  dnssec: true
  domain: symvanta.com
  spf: true
hosts:
- cert_expires: Jan  3 13:14:00 2027 GMT
  host: symvanta.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Symvanta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symvanta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Symvanta
provider_slug: symvanta-com
slug: symvanta-com-domain-security
source_filename: symvanta-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: symvanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 13:14:00 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: symvanta.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: true\n    index:\n    - target: mcp.symvanta.com\n      alpn:\n      - mcp\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/symvanta-com/security/symvanta-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CodeGraph
- AI
- KnowledgeGraph
- MCP
- OpenSource
---
