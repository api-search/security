---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leadersintech.org
  spf: true
hosts:
- cert_expires: Aug 22 21:19:13 2026 GMT
  host: www.leadersintech.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leaders In Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leaders In Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leaders In Tech
provider_slug: leaders-in-tech
slug: leaders-in-tech-domain-security
source_filename: leaders-in-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leadersintech.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:19:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leadersintech.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaders-in-tech/refs/heads/main/security/leaders-in-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Leadership Development
- Executive Education
- Professional Training
- Startups
- Founders
- Coaching
- Community
- Y Combinator
---
