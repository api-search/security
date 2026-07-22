---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: studysoup.com
  spf: true
hosts:
- cert_expires: Oct  4 22:50:57 2026 GMT
  host: studysoup.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Studysoup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StudySoup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: StudySoup
provider_slug: studysoup
slug: studysoup-domain-security
source_filename: studysoup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: studysoup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 22:50:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: studysoup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/studysoup/refs/heads/main/security/studysoup-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Education
- EdTech
- Study Tools
- Students
- Notes
- Learning
---
