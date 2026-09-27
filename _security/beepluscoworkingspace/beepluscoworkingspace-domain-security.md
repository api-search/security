---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beeplus.io
  spf: true
hosts:
- cert_expires: Nov 19 22:38:36 2026 GMT
  host: beeplus.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beepluscoworkingspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beepluscoworkingspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beepluscoworkingspace
provider_slug: beepluscoworkingspace
slug: beepluscoworkingspace-domain-security
source_filename: beepluscoworkingspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beeplus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 22:38:36 2026 GMT\n  hsts: false\ndomains:\n- domain: beeplus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beepluscoworkingspace/refs/heads/main/security/beepluscoworkingspace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agile
- Management
- SaaS
- Brazil
---
