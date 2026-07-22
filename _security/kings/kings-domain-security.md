---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kings.lt
  spf: true
hosts:
- cert_expires: Oct 14 00:32:23 2026 GMT
  host: kings.lt
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Kings
provider_slug: kings
slug: kings-domain-security
source_filename: kings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kings.lt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 00:32:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: kings.lt\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kings/refs/heads/main/security/kings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- Olympiad
- Academic Competition
- Students
- EdTech
---
