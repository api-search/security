---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nexusword.it
  spf: true
hosts:
- cert_expires: Dec 25 13:10:18 2026 GMT
  host: nexusword.it
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NEXUS Word Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NEXUS Word, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NEXUS Word
provider_slug: nexusword-it
slug: nexusword-it-domain-security
source_filename: nexusword-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexusword.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 13:10:18 2026 GMT\n  hsts: false\ndomains:\n- domain: nexusword.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nexusword-it/security/nexusword-it-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Chat
- Workspace
- Beta Service
- Connectors
---
