---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:noc@caffeine.tv"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caffeine.tv
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.caffeine.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caffeine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caffeine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Caffeine
provider_slug: caffeine
slug: caffeine-domain-security
source_filename: caffeine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caffeine.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: caffeine.tv\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:noc@caffeine.tv\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caffeine/refs/heads/main/security/caffeine-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Live Streaming
- Social Broadcasting
- Video
- WebRTC
- Sports
- Gaming
- Entertainment
---
