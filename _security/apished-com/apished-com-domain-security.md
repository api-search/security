---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: apished.com
  spf: true
hosts:
- cert_expires: Jan 14 07:52:15 2027 GMT
  host: apished.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apished Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apished-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: apished-com
provider_slug: apished-com
slug: apished-com-domain-security
source_filename: apished-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apished.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 07:52:15 2027 GMT\n  hsts: null\ndomains:\n- domain: apished.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/apished-com/security/apished-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- API
- Modular
- OpenAPI
- MCP
- Utilities
---
