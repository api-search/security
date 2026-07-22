---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: schoolai.com
  spf: true
hosts:
- cert_expires: Aug 26 15:51:10 2026 GMT
  host: schoolai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schoolai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SchoolAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SchoolAI
provider_slug: schoolai
slug: schoolai-domain-security
source_filename: schoolai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: schoolai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 15:51:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: schoolai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schoolai/refs/heads/main/security/schoolai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Education
- EdTech
- Learning
- Teachers
- K-12
- Higher Education
---
