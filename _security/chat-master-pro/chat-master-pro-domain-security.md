---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chat-master.pro
  spf: true
hosts:
- cert_expires: Nov 29 02:23:53 2026 GMT
  host: chat-master.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chat Master Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chat Master, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chat Master
provider_slug: chat-master-pro
slug: chat-master-pro-domain-security
source_filename: chat-master-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chat-master.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 02:23:53 2026 GMT\n  hsts: false\ndomains:\n- domain: chat-master.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/chat-master-pro/security/chat-master-pro-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
