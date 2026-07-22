---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uplevelteam.com
  spf: true
hosts:
- cert_expires: Aug 22 06:46:47 2026 GMT
  host: uplevelteam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uplevelteam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uplevel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Uplevel
provider_slug: uplevelteam
slug: uplevelteam-domain-security
source_filename: uplevelteam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uplevelteam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:46:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uplevelteam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplevelteam/refs/heads/main/security/uplevelteam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Engineering Intelligence
- Developer Productivity
- Developer Experience
- DORA Metrics
- Software Engineering
- Analytics
- SaaS
---
