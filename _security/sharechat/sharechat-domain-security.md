---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sharechat.com
  spf: true
hosts:
- cert_expires: Mar  7 06:48:49 2027 GMT
  host: sharechat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sharechat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sharechat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sharechat
provider_slug: sharechat
slug: sharechat-domain-security
source_filename: sharechat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sharechat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 06:48:49 2027 GMT\n  hsts: false\ndomains:\n- domain: sharechat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharechat/refs/heads/main/security/sharechat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Social Media
- Social Network
- Short Video
- User Generated Content
- Content Sharing
- Advertising
- India
- Regional Language
---
