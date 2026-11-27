---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: endlessai.org
  spf: true
hosts:
- cert_expires: Feb  3 08:39:09 2027 GMT
  host: endlessai.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Endless Whiteboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endless Whiteboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Endless Whiteboard
provider_slug: endlessai-org
slug: endlessai-org-domain-security
source_filename: endlessai-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: endlessai.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:39:09 2027 GMT\n  hsts: false\ndomains:\n- domain: endlessai.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/endlessai-org/security/endlessai-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Whiteboard
- Collaboration
- Productivity
- Cross-Platform
- Drawing
---
