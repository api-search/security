---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: internmatch.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: internmatch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Looksharp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LookSharp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LookSharp
provider_slug: looksharp
slug: looksharp-domain-security
source_filename: looksharp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: internmatch.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: internmatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looksharp/refs/heads/main/security/looksharp-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Jobs
- Recruiting
- Internships
- Careers
- Education
- Marketplace
- Human Resources
---
