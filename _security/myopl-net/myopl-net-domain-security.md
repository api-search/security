---
api_specs:
- filename: myopl-net-mcp-api-openapi.yml
  format: yaml
  label: myopl-net MCP API
  slug: myopl-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopl-net/openapi/myopl-net-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: myopl.net
  spf: true
hosts:
- cert_expires: Jan 18 13:36:01 2027 GMT
  host: myopl.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Myopl Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for myopl-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: myopl-net
provider_slug: myopl-net
slug: myopl-net-domain-security
source_filename: myopl-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myopl.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 13:36:01 2027 GMT\n  hsts: false\ndomains:\n- domain: myopl.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/myopl-net/security/myopl-net-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Pickleball
- Sports
- Community
- Platform
---
