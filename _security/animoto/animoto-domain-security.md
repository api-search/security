---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: animoto.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: animoto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Animoto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Animoto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Animoto
provider_slug: animoto
slug: animoto-domain-security
source_filename: animoto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: animoto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: animoto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/animoto/refs/heads/main/security/animoto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Video
- Video Creation
- Video Editing
- Slideshow
- Marketing
- Social Media
- Content Creation
- SaaS
---
