---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biome.co.jp
  spf: true
hosts:
- cert_expires: Dec 21 03:23:40 2026 GMT
  host: biome.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biomejapan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biomejapan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biomejapan
provider_slug: biomejapan
slug: biomejapan-domain-security
source_filename: biomejapan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biome.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 03:23:40 2026 GMT\n  hsts: false\ndomains:\n- domain: biome.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biomejapan/refs/heads/main/security/biomejapan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Ecology
- Sustainability
- Japan
---
