---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: structura.tools
  spf: false
hosts:
- cert_expires: Jan  3 11:16:47 2027 GMT
  host: structura.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Structura Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Structura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Structura
provider_slug: structura-tools
slug: structura-tools-domain-security
source_filename: structura-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: structura.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 11:16:47 2027 GMT\n  hsts: false\ndomains:\n- domain: structura.tools\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/structura-tools/security/structura-tools-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Code Generation
- Domain Modeling
- UML
- Software Architecture
- Low-Code
- Compliance
- MCP
---
