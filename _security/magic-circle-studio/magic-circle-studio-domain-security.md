---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magiccircle.studio
  spf: true
hosts:
- cert_expires: Sep 20 23:55:42 2026 GMT
  host: www.magiccircle.studio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magic Circle Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic Circle Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Magic Circle Studio
provider_slug: magic-circle-studio
slug: magic-circle-studio-domain-security
source_filename: magic-circle-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.magiccircle.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:55:42 2026 GMT\n  hsts: false\ndomains:\n- domain: magiccircle.studio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-circle-studio/refs/heads/main/security/magic-circle-studio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Games
- Gaming
- Mobile Games
- Consumer
- Social Games
- Entertainment
---
