---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: castbox.fm
  spf: true
hosts:
- cert_expires: Oct 13 12:13:50 2026 GMT
  host: castbox.fm
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Castboxapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Castbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Castbox
provider_slug: castboxapp
slug: castboxapp-domain-security
source_filename: castboxapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: castbox.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 12:13:50 2026 GMT\n  hsts: false\ndomains:\n- domain: castbox.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castboxapp/refs/heads/main/security/castboxapp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Podcasts
- Audio
- Media
- Streaming
- Podcasting
- Content
- Consumer
---
