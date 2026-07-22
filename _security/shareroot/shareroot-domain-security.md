---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shareroot.co
  spf: false
hosts:
- cert_expires: Sep  1 13:37:40 2026 GMT
  host: shareroot.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shareroot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShareRoot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ShareRoot
provider_slug: shareroot
slug: shareroot-domain-security
source_filename: shareroot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shareroot.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:37:40 2026 GMT\n  hsts: false\ndomains:\n- domain: shareroot.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shareroot/refs/heads/main/security/shareroot-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Marketing
- Social Media
- User Generated Content
- Digital Experience
- Advertising
---
