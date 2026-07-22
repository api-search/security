---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: volta-xr.com
  spf: true
hosts:
- cert_expires: Oct 14 22:52:11 2026 GMT
  host: volta-xr.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Volta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Volta
provider_slug: volta
slug: volta-domain-security
source_filename: volta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volta-xr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:52:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: volta-xr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volta/refs/heads/main/security/volta-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Experiential Technology
- Live Events
- Audience Engagement
- Interactive Experiences
- Out-of-Home Advertising
- Event Technology
- Extended Reality
---
