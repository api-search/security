---
api_specs:
- filename: proctorio-openapi.yml
  format: yaml
  label: Proctorio Launch API (v2)
  slug: proctorio-launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proctorio/refs/heads/main/openapi/proctorio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: proctorio.com
  spf: true
hosts:
- cert_expires: Aug 14 03:01:45 2026 GMT
  host: proctorio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proctorio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proctorio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Proctorio
provider_slug: proctorio
slug: proctorio-domain-security
source_filename: proctorio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: proctorio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:01:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: proctorio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proctorio/refs/heads/main/security/proctorio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Online Proctoring
- Remote Proctoring
- Exam Integrity
- Assessment
- EdTech
- LTI
- LMS Integration
- Learning Integrity
---
