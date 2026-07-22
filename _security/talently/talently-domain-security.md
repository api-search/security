---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: talently.tech
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: talently.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talently Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talently, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Talently
provider_slug: talently
slug: talently-domain-security
source_filename: talently-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talently.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: talently.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talently/refs/heads/main/security/talently-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Recruiting
- Talent Marketplace
- Hiring
- Jobs
- Tech Talent
- LATAM
---
