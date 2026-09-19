---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agripedia.co.jp
  spf: false
hosts:
- cert_expires: Nov 12 07:20:29 2026 GMT
  host: agripedia.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agripedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agripedia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Agripedia
provider_slug: agripedia
slug: agripedia-domain-security
source_filename: agripedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agripedia.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:20:29 2026 GMT\n  hsts: false\ndomains:\n- domain: agripedia.co.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agripedia/refs/heads/main/security/agripedia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agriculture
- AgTech
- Farm Management
- Food Supply Chain
- Traceability
- GAP Certification
- B2B Marketplace
- Japan
---
