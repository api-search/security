---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: entrino.net
  spf: true
hosts:
- cert_expires: Nov 20 18:32:25 2026 GMT
  host: entrino.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Entrino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entrino.net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Entrino.net
provider_slug: entrino
slug: entrino-domain-security
source_filename: entrino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: entrino.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 18:32:25 2026 GMT\n  hsts: false\ndomains:\n- domain: entrino.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entrino/refs/heads/main/security/entrino-domain-security.yml
summary_line: TLSv1.3
tags:
- Access Control
- EventManagement
- Security
- Software-as-a-Service
- Entrino
---
