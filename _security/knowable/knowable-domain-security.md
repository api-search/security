---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: knowable.fyi
  spf: false
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: knowable.fyi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knowable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knowable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Knowable
provider_slug: knowable
slug: knowable-domain-security
source_filename: knowable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knowable.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: knowable.fyi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knowable/refs/heads/main/security/knowable-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Audio
- Learning
- Education
- Media
- Podcasting
- Online Courses
- Consumer
- Defunct
- a16z Portfolio
---
