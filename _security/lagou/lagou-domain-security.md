---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lagou.com
  spf: true
hosts:
- cert_expires: Dec 11 02:31:45 2026 GMT
  host: lagou.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lagou Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lagou, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lagou
provider_slug: lagou
slug: lagou-domain-security
source_filename: lagou-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lagou.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 02:31:45 2026 GMT\n  hsts: false\ndomains:\n- domain: lagou.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lagou/refs/heads/main/security/lagou-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Recruitment
- Jobs
- Hiring
- Human Resources
- Talent
- Careers
- Employment
- Education
- China
---
