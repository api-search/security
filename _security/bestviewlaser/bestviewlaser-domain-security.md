---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bvlaser.com
  spf: true
hosts:
- cert_expires: Nov 19 18:06:56 2026 GMT
  host: www.bvlaser.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bestviewlaser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bestviewlaser, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bestviewlaser
provider_slug: bestviewlaser
slug: bestviewlaser-domain-security
source_filename: bestviewlaser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bvlaser.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 18:06:56 2026 GMT\n  hsts: false\ndomains:\n- domain: bvlaser.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bestviewlaser/refs/heads/main/security/bestviewlaser-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Medical
- Aesthetic
- Lasers
- Manufacturing
---
