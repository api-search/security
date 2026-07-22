---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: about.me
  spf: true
hosts:
- cert_expires: Oct  1 03:20:18 2026 GMT
  host: about.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aboutme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for About.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: About.me
provider_slug: aboutme
slug: aboutme-domain-security
source_filename: aboutme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: about.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:20:18 2026 GMT\n  hsts: false\ndomains:\n- domain: about.me\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aboutme/refs/heads/main/security/aboutme-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Personal Website
- Online Identity
- Profile Page
- Personal Branding
- Website Builder
- Landing Page
- Portfolio
- AI
- Lead Capture
---
