---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bridgewire.cloud
  spf: false
hosts:
- cert_expires: Dec 27 19:09:03 2026 GMT
  host: bridgewire.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bridgewire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridgewire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Bridgewire
provider_slug: bridgewire
slug: bridgewire-domain-security
source_filename: bridgewire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bridgewire.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 19:09:03 2026 GMT\n  hsts: false\ndomains:\n- domain: bridgewire.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridgewire/refs/heads/main/security/bridgewire-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Messaging
- Automation
- Integration
- Communications
---
