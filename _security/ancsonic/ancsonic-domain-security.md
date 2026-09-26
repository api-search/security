---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ancsonic.com
  spf: false
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.ancsonic.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ancsonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ancsonic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ancsonic
provider_slug: ancsonic
slug: ancsonic-domain-security
source_filename: ancsonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ancsonic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ancsonic.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ancsonic/refs/heads/main/security/ancsonic-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Acoustic
- Technology
- Manufacturing
- IoT
---
