---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcp-catalog.ru
  spf: true
hosts:
- cert_expires: Jan 23 11:17:29 2027 GMT
  host: mcp-catalog.ru
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Каталог MCP-серверов по-русски Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Каталог MCP-серверов по-русски, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Каталог MCP-серверов по-русски
provider_slug: mcp-catalog-ru
slug: mcp-catalog-ru-domain-security
source_filename: mcp-catalog-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcp-catalog.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 11:17:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcp-catalog.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mcp-catalog-ru/security/mcp-catalog-ru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Catalog
- Russian
- MCP
- Open Source
---
