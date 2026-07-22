---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usepuddle.com
  spf: true
hosts:
- cert_expires: Oct  6 23:30:35 2026 GMT
  host: usepuddle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Puddle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puddle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Puddle
provider_slug: puddle
slug: puddle-domain-security
source_filename: puddle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usepuddle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:30:35 2026 GMT\n  hsts: false\ndomains:\n- domain: usepuddle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puddle/refs/heads/main/security/puddle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technical Interviews
- Hiring
- Developer Assessment
- Recruiting
- AI
- Coding Assessment
---
