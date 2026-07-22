---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zhipin.com
  spf: true
hosts:
- cert_expires: Sep 23 02:48:07 2026 GMT
  host: zhipin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Boss
provider_slug: boss
slug: boss-domain-security
source_filename: boss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zhipin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:48:07 2026 GMT\n  hsts: false\ndomains:\n- domain: zhipin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boss/refs/heads/main/security/boss-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Technology
- Recruitment
- Human Resources
- Jobs
- Hiring
- Talent
- Marketplace
---
