---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: better-design.com
  spf: true
hosts:
- cert_expires: Jan 31 00:12:08 2027 GMT
  host: better-design.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Better Design Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Better Design, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Better Design
provider_slug: better-design-com
slug: better-design-com-domain-security
source_filename: better-design-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: better-design.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 00:12:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: better-design.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/better-design-com/security/better-design-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Design
- Artificial Intelligence
- Components
- MCP
- UI
---
