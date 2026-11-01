---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: humanmcp.net
  spf: false
hosts:
- cert_expires: Jan 25 05:14:50 2027 GMT
  host: humanmcp.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Humanmcp Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for humanmcp-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: humanmcp-net
provider_slug: humanmcp-net
slug: humanmcp-net-domain-security
source_filename: humanmcp-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanmcp.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 05:14:50 2027 GMT\n  hsts: false\ndomains:\n- domain: humanmcp.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/humanmcp-net/security/humanmcp-net-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Human
- MCP
- API
- OpenAPI
---
