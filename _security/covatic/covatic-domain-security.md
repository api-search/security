---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: covatic.com
  spf: true
hosts:
- cert_expires: Sep  4 12:29:30 2026 GMT
  host: covatic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Covatic
provider_slug: covatic
slug: covatic-domain-security
source_filename: covatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: covatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 12:29:30 2026 GMT\n  hsts: false\ndomains:\n- domain: covatic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/security/covatic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising Technology
- AdTech
- Audience Intelligence
- Data Management Platform
- Connected TV
- Privacy
- On-Device Processing
- Attribution
- Audio
---
