---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tagged.com
  spf: true
hosts:
- cert_expires: Aug 22 21:42:55 2026 GMT
  host: www.tagged.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tagged Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tagged, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tagged
provider_slug: tagged
slug: tagged-domain-security
source_filename: tagged-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tagged.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:42:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tagged.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tagged/refs/heads/main/security/tagged-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Network
- Social Discovery
- Online Dating
- Consumer
- Messaging
- Mobile App
---
