---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: daredrop.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: daredrop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dare Drop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dare Drop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dare Drop
provider_slug: dare-drop
slug: dare-drop-domain-security
source_filename: dare-drop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daredrop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: daredrop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dare-drop/refs/heads/main/security/dare-drop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Influencer Marketing
- Content Creators
- Streaming
- Twitch
- YouTube
- TikTok
- Marketing
---
