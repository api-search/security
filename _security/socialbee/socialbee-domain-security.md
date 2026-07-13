---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: socialbee.com
  spf: true
hosts:
- cert_expires: Sep 23 22:30:53 2026 GMT
  host: socialbee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 00:40:58 2026 GMT
  host: app.socialbee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Socialbee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SocialBee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SocialBee
provider_slug: socialbee
slug: socialbee-domain-security
source_filename: socialbee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: socialbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:30:53 2026 GMT\n  hsts: false\n- host: app.socialbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:40:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: socialbee.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socialbee/refs/heads/main/security/socialbee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Social Media Management
- Content Scheduling
- Content Recycling
- Social Media Analytics
- AI Caption Generation
---
