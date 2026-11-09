---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: auseconmcp.com
  spf: false
hosts:
- cert_expires: Dec 14 05:27:29 2026 GMT
  host: auseconmcp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auseconmcp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Economic Data MCP Server, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Australian Economic Data MCP Server
provider_slug: auseconmcp-com
slug: auseconmcp-com-domain-security
source_filename: auseconmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auseconmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 05:27:29 2026 GMT\n  hsts: null\ndomains:\n- domain: auseconmcp.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/auseconmcp-com/security/auseconmcp-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Finance
- Data
- Australia
- MCP
- Economics
---
