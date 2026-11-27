---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mcp.film
  spf: true
hosts:
- cert_expires: Jan 22 22:04:49 2027 GMT
  host: mcp.film
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mcp.film Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mcp.film, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: mcp.film
provider_slug: mcp-film
slug: mcp-film-domain-security
source_filename: mcp-film-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcp.film\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 22:04:49 2027 GMT\n  hsts: false\ndomains:\n- domain: mcp.film\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcp-film/security/mcp-film-domain-security.yml
summary_line: TLSv1.3
tags:
- Directory
- AI Filmmaking
- MCP
- Video Generation
- Voice
- Music
- Editing
- Studio
---
