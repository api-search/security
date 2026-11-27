---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: colabro.app
  spf: true
hosts:
- cert_expires: Jan  2 20:37:48 2027 GMT
  host: colabro.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: colabro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for colabro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: colabro
provider_slug: colabro-app
slug: colabro-app-domain-security
source_filename: colabro-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: colabro.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 20:37:48 2027 GMT\n  hsts: false\ndomains:\n- domain: colabro.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/colabro-app/security/colabro-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Collaboration
- Workspace
- AI Agents
- Productivity
- Team Management
---
