---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firstjob.me
  spf: true
hosts:
- cert_expires: Sep  7 02:33:49 2026 GMT
  host: firstjob.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firstjobme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firstjob.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Firstjob.me
provider_slug: firstjobme
slug: firstjobme-domain-security
source_filename: firstjobme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstjob.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firstjob.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstjobme/refs/heads/main/security/firstjobme-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Jobs
- Recruiting
- Employment
- Career
- Internships
- Human Resources
- Latin America
- Chile
---
