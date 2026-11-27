---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: anacraft.dev
  spf: false
hosts:
- cert_expires: Jan 15 21:01:42 2027 GMT
  host: anacraft.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: anacraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for anacraft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: anacraft
provider_slug: anacraft-dev
slug: anacraft-dev-domain-security
source_filename: anacraft-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anacraft.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 21:01:42 2027 GMT\n  hsts: false\ndomains:\n- domain: anacraft.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/anacraft-dev/security/anacraft-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Analytics
- Google Analytics
- MCP
- Open Source
- Dashboards
- Company
---
