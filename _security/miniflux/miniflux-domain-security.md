---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: miniflux.app
  spf: true
hosts:
- cert_expires: Nov 27 06:49:21 2026 GMT
  host: miniflux.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Miniflux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miniflux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Miniflux
provider_slug: miniflux
slug: miniflux-domain-security
source_filename: miniflux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miniflux.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 06:49:21 2026 GMT\n  hsts: false\ndomains:\n- domain: miniflux.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/security/miniflux-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Feed Reader
- Open Source
- Self-Hosted
- Minimalist
- Privacy
---
