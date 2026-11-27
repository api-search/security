---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coredash.app
  spf: true
hosts:
- cert_expires: Jan 30 06:50:52 2027 GMT
  host: coredash.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CoreDash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreDash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CoreDash
provider_slug: coredash-app
slug: coredash-app-domain-security
source_filename: coredash-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coredash.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 06:50:52 2027 GMT\n  hsts: false\ndomains:\n- domain: coredash.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/coredash-app/security/coredash-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Core Web Vitals
- Real User Monitoring
- Web Performance
- Observability
- MCP
- JSON-RPC
- AI Agents
---
