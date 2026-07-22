---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: projectx.cloud
  spf: false
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.projectx.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Projectx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Projectx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Projectx
provider_slug: projectx
slug: projectx-domain-security
source_filename: projectx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.projectx.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: projectx.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/projectx/refs/heads/main/security/projectx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Operating System
- AI Agents
- GPU
- Compute
- Cloud Computing
- Infrastructure
- Developer Tools
- Y Combinator
---
